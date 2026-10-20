# 阶段快照恢复

Release：https://github.com/shanghaicellcenter/qiming-rocket-opendesign/releases/tag/wip-20261020 。精确附件名、字节数、SHA与公开URL见state/checkpoint.json。当前12归档包均已真实上传并由公开API回读确认；最后小补丁也有实际payload。

## 顺序与校验

1. 全部9个base包：core、original-sources、production-source-voice-01-v2、editable-sources三个分包、legacy-outlined-and-late-voices、native-media-interactive两个分包。
2. qiming-FINAL-portable-overlay-v1.tar.gz（517432571字节，SHA036eb4772628bbab82f200f37aabf02cb574ef4d36bbe9f2b15154c067885fe8）。
3. qiming-AFTER-FINAL-produced-media-delta-v2.tar.gz（58558139字节，SHAe4f608c24fdbee74c42a639ccfa3715488d543f67ebf2bb17331449875d441ea）。
4. qiming-FINAL-small-v3-public.tar.gz最后覆盖；4,069,157字节，SHA256 0e91ece04cd34a8a8cb155444c6a69a5b33f2bbb7faab41b3edf85b22aee31a5。已实际上传；本地108成员核SHA通过，fresh恢复待。

每个包先独立验证归档SHA及其自己的SNAPSHOT_MANIFEST.json，再解压到独立目录核成员；然后按上述顺序叠到共同干净恢复根，同路径以后者覆盖。不能用最后覆盖的一个manifest证明全部包，更不能倒序让旧文件覆盖新修订。全部overlay应用后的合并目录仍需再次核查和实际重开，本轮尚未建立该整体验证。

source-voice-v2包根有recovery-tools/verify_archive_stream.py、recovery-tools/verify_snapshot.py与recovery-tools/restore_workspace_paths.py；不是recovery-tools/packaging目录。可先运行`python3 recovery-tools/verify_archive_stream.py 下载包.tar.gz`，再运行`python3 recovery-tools/verify_snapshot.py 单包独立解压目录`。以各包实际manifest为准。

核完原始hash再对恢复副本运行`python3 recovery-tools/restore_workspace_paths.py 恢复根`做dry-run；检查后才追加`--apply`，只替换${WORKSPACE_ROOT}/${LOCAL_USER_HOME}占位。需要未来远端环境时才传`--remote-user-home`；播放现有媒体不需要连Spark/A800。原Desktop输入从original-sources按清单恢复，不能依赖旧机器绝对路径或软链。

## 打开已有工程

`python3 -m http.server 8080 --directory 恢复根`，再打开`/OpenDesign/project/index.html`、`/OpenDesign/project/course/index.html`及`/outputs/rocket-v2/样章播放器/index.html`。媒体须来自相应包，core不含全部新工作片时不表示core损坏。

core包根有README_RESTORE.md、restore_opendesign_project.py、OpenDesign/project与OpenDesign/metadata。可选的原生应用恢复命令为`python3 restore_opendesign_project.py --snapshot-root 恢复根 --opendesign-data 新命名空间data目录 --new-project-id`，默认dry-run；`--apply`才复制，`--register`才注册且需要现有app.sqlite。本轮未执行数据库注册，不宣称原生应用导入通过；不要覆盖现有项目、全局app.sqlite或账号数据。

## 已证明与尚待证明

- Core：实际公开回下载，815成员SHA与隔离解压通过，5页面资源/JS错误0；应用注册未运行。
- Original-sources：实际公开回下载，385成员写入及重读SHA通过；保留CAD ZIP样本149成员CRC通过。
- Source-voice-v2：实际公开回下载，2344成员写入及重读SHA通过；其中A1-04恢复blend经本机Blender5.2.2只读重开和640×360实际渲染查看，输入SHA不变。
- AFTER-FINAL media delta-v2：实际公开回下载，127成员写入及重读SHA通过，所留SH040视频完整解码通过。
- 其余7个已上传大包、最后小补丁的fresh恢复及同一合并工程重开：fresh验证仍pending。逐包恢复不等于全课程、全部可编辑场景或主观听审通过。

详见state/recovery-evidence中的公开路径占位副本及state/checkpoint.json。续作从work/rocket-v2/full-course-production/production-next-handoff.md、production-ledger.json与curriculum.json进入，具体课读冻结稿、source-feature-matrix、root-preview-review、composition-plan和当前SHA。最终接受项目仍为0。

21份精确当前SHA均已完成1倍速整段离线技术播放（新SYS-A2/A110/A111全帧且0掉帧）；均为静音技术检查，不计主观听审。当前播放器有21卡、170章跳转和424条字幕核查材料。

最后应用的实际补丁：[qiming-FINAL-small-v3-public.tar.gz](https://github.com/shanghaicellcenter/qiming-rocket-opendesign/releases/download/wip-20261020/qiming-FINAL-small-v3-public.tar.gz)。该包已包含旧小tail的必要安全内容；不要下载未发布的v1/v2或无public后缀试包。

恢复入口的版本边界：Release标签wip-20261020仍指初始baseline；GitHub自动生成的Source code(zip/tar.gz)对应旧标签，不能当完整交接。请读取main分支及上列12个实际归档附件。已核对的最终payload交接版本为[e5b3ae6](https://github.com/shanghaicellcenter/qiming-rocket-opendesign/tree/e5b3ae668b024e4b6a3394ef462e1e4929416322)；本段说明随后补于main，不改变12包字节。
