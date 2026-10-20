# 阶段快照恢复

本页提供方法；逐包当前状态及证据时间以state/checkpoint.json为准。12个实际附件的精确URL/字节/SHA在RELEASE_ASSETS.json和SHA256SUMS。Release的自动Source code ZIP对应初始tag，并不含完整交接；读取main与12个真实附件。

## 覆盖顺序

1. 全部9个base：core、original-sources、production-source-voice-01-v2、editable-sources三个分包、legacy-outlined-and-late-voices、native-media-interactive两个分包。
2. qiming-FINAL-portable-overlay-v1.tar.gz。
3. qiming-AFTER-FINAL-produced-media-delta-v2.tar.gz。
4. qiming-FINAL-small-v3-public.tar.gz最后覆盖。该包含旧小tail的必要安全内容；未发布的v1/v2/无public试包不需要。

每包独立核归档SHA和自己的SNAPSHOT_MANIFEST.json全部成员；所有版本按顺序累计最终路径→winning SHA，不能用最后覆盖的单个manifest代表所有包。低优先级base不许盖回已验证的较新overlay。中断写入须留in_progress失败门，解决后才处理别包。独立可写副本可使用APFS写时复制，不能用硬链接让恢复编辑影响原件。

## 验证、路径与打开

source-voice-v2包根提供recovery-tools/verify_archive_stream.py、verify_snapshot.py、restore_workspace_paths.py，不是recovery-tools/packaging目录。先运行`python3 recovery-tools/verify_archive_stream.py 下载包.tar.gz`；单包独立根用`python3 recovery-tools/verify_snapshot.py 单包目录`。这些单包通过不能代替整个合并根检查。

核完原始发布SHA，再对恢复副本运行`python3 recovery-tools/restore_workspace_paths.py 恢复根`做dry-run。检查后才追加`--apply`替换${WORKSPACE_ROOT}/${LOCAL_USER_HOME}占位，并另外记录路径改写后SHA。只有未来确需远端时才显式传--remote-user-home；播放已有媒体不需要Spark/A800。原Desktop输入由original-sources恢复，不依赖旧机器路径或软链。

在合并根提供HTTP：`python3 -m http.server 8080 --directory 恢复根`。实际检查/OpenDesign/project/index.html、/OpenDesign/project/course/index.html、/outputs/rocket-v2/样章播放器/index.html，以及主图册、原理实验、原生模型、21视频/全部下载源链接。浏览器/手机/离线/源可编辑各自记录范围；不以技术播放推定主观听审。

core根有README_RESTORE.md、restore_opendesign_project.py、OpenDesign/project与OpenDesign/metadata。可选原生应用恢复：`python3 restore_opendesign_project.py --snapshot-root 恢复根 --opendesign-data 新命名空间data目录 --new-project-id`默认dry-run；--apply才复制，--register才注册且需现有app.sqlite。本轮没有注册数据库，不能写原生应用导入通过；不要覆盖现有项目、全局数据库或账号数据。

## 验收与续作边界

完整合并工程恢复仍未验收。部分单包公开下载、逐成员SHA、单文件重开/64旧文件只读重开和选定视频解码是狭义证据，不能扩成全工程或课程验收。最新原始回执及逐项缺口见state/recovery-evidence/postdeadline-recovery。

当前phase为restore_and_bounded_cleanup_only。继续实际恢复队列和安全临时清理；完整课程的69批/1156规划动作仅作以后制作安排，不自动启动新配音或新GPU。原件与唯一源保留，实际主观视听/完整逐件/组装/QC/实物适用性都保持各自未完成状态。
