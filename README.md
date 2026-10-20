# 启明火箭 · OpenDesign 中文互动科普

**制作中的阶段存档（WIP），不是整套课程完成版。**

面向没有火箭工程基础的读者，以原始资料、可编辑三维场景、互动页面和中文讲解说明部件、原理及系统关系。既定范围为172条物料、34项定制件、9个系统、8类原理与3个综合过渡，共226章、至少1156个计划教学动作。组装、检查、仿真及实测证据仍属于完整目标。

当前保存21段有声工作核查稿，共1901.125秒（31分41.125秒）。其中SYS-A2为248.791667秒，A1-10为94秒，A1-11为83.25秒。**完整接受的BOM、定制件和系统均为0；实际听审与连续主观验收未通过。** 自动转写、PCM连续性、解码、离散画面和静音技术播放不能代替这些验收。

用户要求于2026-10-20 04:17:38 UTC前保存可继续的进度，即使课程尚未完成。[GitHub Release](https://github.com/shanghaicellcenter/qiming-rocket-opendesign/releases/tag/wip-20261020)当前公开API已确认12个归档包的大小与SHA，包括FINAL portable overlay和AFTER-FINAL delta-v2；最后小补丁qiming-FINAL-small-v3-public.tar.gz也已实际上传并回读大小/SHA。精确状态见[state/checkpoint.json](state/checkpoint.json)。

已从公开Release重新下载并逐成员核对core815项、原资料385项、source-voice2344项。媒体补充包127项亦已重新下载、逐项写入复读校验并抽取视频完整解码；Core五个隔离页面资源/JS错误为0；恢复的A1-04可编辑文件已在Blender5.2.2只读重开并实际渲染查看。其余包的fresh恢复及同一合并目录整体重开仍待验证，不能把四包或单文件验证扩大为全工程验收。

继续前阅读[AI_HANDOFF.md](AI_HANDOFF.md)和[RESTORE.md](RESTORE.md)。恢复顺序必须是全部base包→FINAL portable overlay→AFTER-FINAL delta-v2→qiming-FINAL-small-v3-public.tar.gz。先逐包验证，再合并覆盖；不能只克隆代码就认为大文件已恢复。

本项目保留原作者、许可、CAD身份与来源。软件、原资料、CAD、生成语音和混合视频的许可层次分别查看随包条款；技术演示不作硬件性能认证。

21份精确当前SHA均已完成1倍速整段离线技术播放（新SYS-A2/A110/A111全帧且0掉帧）；均为静音技术检查，不计主观听审。当前播放器有21卡、170章跳转和424条字幕核查材料。

最后应用的实际补丁：[qiming-FINAL-small-v3-public.tar.gz](https://github.com/shanghaicellcenter/qiming-rocket-opendesign/releases/download/wip-20261020/qiming-FINAL-small-v3-public.tar.gz)。该包已包含旧小tail的必要安全内容；不要下载未发布的v1/v2或无public后缀试包。

恢复入口的版本边界：Release标签wip-20261020仍指初始baseline；GitHub自动生成的Source code(zip/tar.gz)对应旧标签，不能当完整交接。请读取main分支及上列12个实际归档附件。已核对的最终payload交接版本为[e5b3ae6](https://github.com/shanghaicellcenter/qiming-rocket-opendesign/tree/e5b3ae668b024e4b6a3394ef462e1e4929416322)；本段说明随后补于main，不改变12包字节。
