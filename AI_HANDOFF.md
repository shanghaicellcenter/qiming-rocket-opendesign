# 给下一位AI的续作交接

这是WIP阶段存档。21段有声核查稿共1901.125秒，所有226章仍未完成最终验收；accepted BOM/custom/systems均为0。先读state/checkpoint.json、state/backlog.json与RESTORE.md。早包中的台账可能较旧，以按规定顺序应用后的最后checkpoint和逐附件manifest为准。

## 固定要求

中文互动工程和中文讲解视频都要，外行需看懂每个部件、局部、相邻关系、原理变化及理解检查。范围172 BOM、34定制件、9系统、8原理与3综合过渡。展示名用启明火箭，原作者/许可/来源身份保留。使用Blender/OpenDesign/Machine，不用Higgsfield或LibTV。Blender先读expert，再读相关相邻专业技能；13技能目录保持相邻。

有真实CAD或装配就使用原几何与正确位置；原料保持原料；教学剖视、独立原理、放大和颜色必须说明性质。不要把静态资产或计划动作记成已完成动画，也不把演示当制造/安装/性能认证。

## 当前断点

已保存旧18稿，加SYS-A2 248.791667秒、A1-10 94秒、A1-11 83.25秒，共21稿。当前SYS-A2视频SHA为302b78ffb2fecf71c9edf9d782a005e7fd9aef88c0a2e5b1e25f8a39b31b1a7e；首次63251稿仅作历史问题证据。19源片、SH050标签修订、105动作合同及同音编排已留存，重复思考提示修复已编码。A110当前SHA c111bfee21c143b7ecab30203d59a90ed11d58b22ddeb24c42b0fb5dd4d66ae3，A111当前SHA169509b116c5e1a7e93e67a451b7f0dc3d20eda68402708eaf7ff3cf9afa5b28。不要沿用旧“尚未合成”的状态。

35条native原声已带回，另5条joined派生不计新原声。保持已确认的Breeze声线与音量：参考SHA b877cfd2a4b951b77e07743a4e569ecca2f3a62e4d990b0b4f2baaaffcd0191f、seed42/CFG1、整段生成；已批准的柔和压缩和每段固定增益约-22.303dBFS方向不需重问。现有声音不变调、不变速，数字零仅插于有PCM证据的真实空白。23秒原PCM独立ASR窗口已解决A110长转写分块重复，不重录。没有宣称本机可继续推理；恢复现有素材不需要Spark/A800。

## 发布与恢复实态

公开API确认12个归档包；FINAL portable overlay517432571字节/SHA036eb4772628bbab82f200f37aabf02cb574ef4d36bbe9f2b15154c067885fe8已确认。最后小补丁qiming-FINAL-small-v3-public.tar.gz已实际上传并回读大小/SHA；本地108成员流式校验通过，fresh回下载仍待。四个包已fresh公开回下载与全成员复核：core815、original385、sourcevoice2344、媒体delta127。其余7个已上传包的fresh恢复仍pending，同一合并工程重开尚未证明。

恢复A1-04文件SHA902b82464d67f8dfff323c56952e66b65598ab26468d62c81d974aeb3478777f已在Blender5.2.2独立只读重开：6景/6相机、0字体对象/字体数据块、0缺失运行依赖；640×360图实际查看非空白，输入SHA/mtime/大小未改。只证明这一恢复成员，不能代替完整课程或听审。

64个旧editable发布副本完成字体程序清除、554活字转等几何轮廓；原件未改。最终语义不变量通过，初次session_uid瞬态失败及修正诊断保留，不声称完整初始日志仍在。历史绝对路径由FINAL portable overlay处理；${WORKSPACE_ROOT}溯源字符串不一定是运行依赖。不要混淆原件SHA与发布副本SHA。

## 续作边界

按69批台账、逐项源证据、特征覆盖、逐句动作合同与精确当前SHA续作；不要重录/重渲已有资产。所有带声片仍是核查稿。原声方向的用户确认不是逐条接受；独立ASR/PCM/解码/技术播放/离散图不能填主观听审和连续内容门。

已回收的是可从保留源/片重建的临时PNG和可重建发布tar；被删PNG字节没有云备份。唯一原资料、可编辑工程、原声和视频保留。不要把删掉的proof栅格称为仍存在，也不要删除其他项目、Desktop原资料、共享技能/工具、全局数据库或远端服务。

21份精确当前SHA均已完成1倍速整段离线技术播放（新SYS-A2/A110/A111全帧且0掉帧）；均为静音技术检查，不计主观听审。当前播放器有21卡、170章跳转和424条字幕核查材料。

最后应用的实际补丁：[qiming-FINAL-small-v3-public.tar.gz](https://github.com/shanghaicellcenter/qiming-rocket-opendesign/releases/download/wip-20261020/qiming-FINAL-small-v3-public.tar.gz)。该包已包含旧小tail的必要安全内容；不要下载未发布的v1/v2或无public后缀试包。
