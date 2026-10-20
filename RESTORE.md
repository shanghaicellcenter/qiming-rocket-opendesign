# 阶段快照恢复入口（准确成员路径，供publisher合并）

仓库是 https://github.com/shanghaicellcenter/qiming-rocket-opendesign ，Release标签为wip-20261020。先读state/checkpoint.json与backlog.json，按实际附件URL下载。截至03:08已确认4个主包真实上传，共1,690,255,232字节（含metadata为1,691,398,299字节）：core、original-sources、production-source-voice-v2与editable01。editable02/03、legacy/late-voice及native_media两包（515,037,321和115,486,589字节）已在本地生成，远端上传尚未确认；必须等真实上传清单，不猜附件名或使用LFS指针。

1. 对每个实际下载包核精确字节/SHA。每包含自己的 SNAPSHOT_MANIFEST.json，先独立验证其成员，再叠到共同干净恢复根；不要把最后覆盖的单个manifest当全部包覆盖证明。
2. 已核packlist：core包根含 README_RESTORE.md、restore_opendesign_project.py、OpenDesign/project/ 与 OpenDesign/metadata/。source-voice-v2包根含 recovery-tools/verify_archive_stream.py、recovery-tools/verify_snapshot.py、recovery-tools/restore_workspace_paths.py。**不是recovery-tools/packaging路径**；后续增量可能另有副本，以对应清单为准。
3. 可流式核包：`python3 recovery-tools/verify_archive_stream.py 下载包.tar.gz`；会写同目录小型manifest/校验回执。对单包独立解压根可用 `python3 recovery-tools/verify_snapshot.py 单包解压目录`。校验完成再做下面路径改写，避免改写后与原hash混淆。
4. 恢复源包后，先运行 `python3 recovery-tools/restore_workspace_paths.py 恢复根` 做dry-run，再按检查结果追加 `--apply`，只改恢复副本中的 `${WORKSPACE_ROOT}`/`${LOCAL_USER_HOME}`占位。需要未来远端环境时才显式传 `--remote-user-home`；不要为了播放现有媒体连接Spark/A800。原Desktop输入应从original-sources包按清单恢复，不能仍依赖旧机绝对路径/OCR软链。
5. 在恢复根提供HTTP：`python3 -m http.server 8080 --directory 恢复根`。打开 `/OpenDesign/project/index.html`、`/OpenDesign/project/course/index.html`。当前独立动态样章播放器的已知工程路径为 `outputs/rocket-v2/样章播放器/index.html`，只有对应媒体包真实上传/恢复后才能打开；core不包含全部新工作片时不要误判为缺包损坏。
6. 接续制作入口：`work/rocket-v2/full-course-production/production-next-handoff.md`、`production-ledger.json`、`curriculum.json`；具体pilot的narration-root-v1、source-feature-matrix、root-preview-review、narrated/composition-plan与精确SHA。随早包的台账可能早于最新增量，须和本次CURRENT_CHECKPOINT及对应最新manifest合并判断，不倒退已修状态。

原生应用恢复为可选：`python3 restore_opendesign_project.py --snapshot-root 恢复根 --opendesign-data 新建或已初始化的OpenDesign命名空间data目录 --new-project-id` 默认dry-run。`--apply`复制项目，`--register`才会注册安全元数据且要求现有app.sqlite；本轮没有执行数据库注册，不可写“应用导入通过”。不要覆盖现有项目、全局app.sqlite或账号数据。

Core实际恢复凭据：177,719,360字节，SHA256 `0305c3fc791ff5f9edaac75181db112a68d86fd0fcf2144930a4857922d1ca67`；815成员真实公开回下载后哈希通过，5隔离页面资源/JS错误0。只能接受core字节/网页恢复，不接受全阶段媒体、工程编辑、真实听感或硬件性能。

当前逐包真实状态以 state/checkpoint.json 为准；最后metadata/source和媒体增量必须按最新清单覆盖同路径。
