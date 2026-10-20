# 给下一位AI的续作交接

当前phase为`restore_and_bounded_cleanup_only`。三小时制作窗口已结束，禁止从旧69批指令自动启动新章节、TTS、Spark/A800或本地课程渲染。`FULL226_COURSE`为`deferred_requires_user_resume`；完整目标没有缩减，也没有完成。现有恢复队列可继续，原件保留。

## 目标与当前缺口

交付应为外行能懂的中文互动工程与中文视频：每项部件外形、细节、位置、连接、作用和原理变化；逐步组装片、逐环节QC与虚拟对齐；仿真平台实跑与适用边界。范围172BOM、34custom、9系统、8原理与3整体/过渡，共226章。

现有21份独立pilot核查稿1901.125秒，并不等于对应canonical章完整接受。完整BOM/custom/systems接受数0；独立动态课程仍缺155物料、34custom、5系统和8canonical原理。静态图册与规划1156动作不是完整动态课。所有当前SHA/逐项缺口见checkpoint与state/recovery-evidence/postdeadline-recovery/requirements-evidence-audit.md。

## 固定制作约束

展示名启明火箭，来源身份/作者/许可/原URL与原件哈希保留。用Blender/OpenDesign/Machine，禁Higgsfield和LibTV。Blender先读expert及相关相邻技能，13目录保持相邻。有真实CAD就保留原几何与原位；原料、局部原理图、示意流动与实物分开标明，不冒充配合/压力/强度/飞行认证。

保持既定Spark Breeze声线/音量，参考SHA b877cfd2a4b951b77e07743a4e569ecca2f3a62e4d990b0b4f2baaaffcd0191f，seed42/CFG1；整段原生生成，2:1软压缩后按段固定增益约-22.303dBFS。不变调/变速，已有35native+5joined不重录；方向批准不代表21片逐条实际听审。23秒独立原PCM识别窗口已解决A110长ASR分块歧义。实际听审/连续主观内容门不能由ASR、PCM、静音播放或离散图填写。

## 精确锁定与恢复入口

SYS-A2当前302b78ffb2fecf71c9edf9d782a005e7fd9aef88c0a2e5b1e25f8a39b31b1a7e，248.791667秒；保留19源/105动作及SH050修订源，首次63251仅历史问题证据。A110当前c111bfee21c143b7ecab30203d59a90ed11d58b22ddeb24c42b0fb5dd4d66ae3，94秒；A111当前169509b116c5e1a7e93e67a451b7f0dc3d20eda68402708eaf7ff3cf9afa5b28，83.25秒。原声和源文件不要从旧状态重复生成。

12实际附件及覆盖顺序见RELEASE_ASSETS.json、SHA256SUMS、RESTORE.md；GitHub自动source ZIP对应旧tag，读取main及真实附件。先验证每个归档/成员，再按覆盖优先级构成一个独立恢复根；同一目录的最终文件须匹配累计winner表。核原始发布SHA后才能改恢复副本中的路径占位，并记录改写后的SHA；不要把原件SHA与清路径/转字体发布SHA混用。

本地当前恢复工具/状态在work/rocket-recovery-20261020/。一个队列下载03→media02→editable02→media01→FINAL→original→voice→delta；另一个已确认的editable01断点writer由root持有，不能重复启动。队列按实际进程/锁/句柄判断活性；超时不等于终止。inProgressArchive未解决时不得跨包。所有最终页面、21视频与可编辑源在同一恢复根实际测试以前，整体恢复保持pending。

组装母片存在但旧跨项目来源路径不可达，可编辑生成源尚未定位；已向用户授权交流的Anatomy chat只索取既有发布位置。不要把文件名检索未见.blend写成某.blend已丢失。原生浏览位置不代表全部接口配合/干涉/公差/承载已验证。

## 证据、许可和删除边界

仿真原案例与作者历史有证据，但没有本次新实物制造、计量校准/原始DAQ/飞行闭环；L858表格与L1018 ORK不是同基线认证。不要宣称本次复现火箭已获真实适用性或安全认证。

已删除的只是有清单/远端大小SHA/可重建输入/无占用证明的临时tar与已记录可重建缓存。旧PNG字节有部分未备份，不能称全部原proof栅格仍可打开。保留原资料、独有生产源、原音、视频、Desktop、共享技能/应用、其他项目及远端环境。整体恢复/依赖未验证不得删除唯一源。不得覆盖全局app.sqlite或账号数据。Breeze语音/混合视频研究非商业层独立于软件许可。
