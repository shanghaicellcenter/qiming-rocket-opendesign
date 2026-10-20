# 启明火箭：恢复核查与要求证据审计

审计时间：2026-10-20T04:41:39.923898+00:00；repo HEAD `aa7934b732784819e3febf3791680de073996f8b`。

已保存WIP、静态全清单和21带声样章；完整课程、完整合并恢复、主观视听及本次实物有效性均未验收。

本轮只读现有文件、计算SHA、读取媒体元数据并核对旧收据。没有启动远端、渲染、配音、下载或新增内容；没有重新主观听审或全片视觉验收。

**当前phase：restore_and_bounded_cleanup_only。入口只继续已发布内容恢复与限定临时文件清理；下列课程缺项是以后阶段待办，本轮不启动新课程、TTS、渲染、Spark/A800。**

状态含义：**proven**＝所述狭义命题已支持；**incomplete**＝有直接进展但门未完；**indirect**＝相关/历史证据；**missing**＝本次范围内缺直接成品或验证。

## 最先影响外行看懂与完整交付的缺项

- P0：6大包尚无fresh成员复核（最后小包108成员、legacy154成员已有），最终合并工程未恢复验证；禁止把已上传当可独立恢复通过。
- P1：155物料/34定制件/5系统/8canonical原理缺独立完整带声动态课。
- P1：现21片实际听审/连续主观视听未过；初心者能否认清每特征、连接与因果尚不能由ASR或解码保证。
- P1：逐组归位无声/未验收且旧编辑源引用不可达；缺完整逐接口解释和阶段QC。
- P1：原位置可见，但没有全接口配合/干涉/版本数量闭环；地面工具不能都留在飞行总装。
- P2：全量curriculum自动句分配是计划，不是逐句语义冻结；缺课需先做术语解释/特征覆盖/真实细节镜头。
- P2：软件案例确运行、原作者家族确有试验史；缺本次实物与对应原始测量，不能宣称新复现真实有效。

## 要求逐项结论

| 要求 | 状态 | 当前证据与缺口 |
|---|---|---|
| R01 完整范围清点与可续作制作计划 | proven | canonical确有172物料、34定制件、9系统、8原理，共226场景（另3开篇/转场）。规划1156独立子镜与69批次。 **缺口/限界：**这是清单与计划存在的证明，不是1156镜或226课程已制作、文本逐字审核已通过。 |
| R02 172物料外形、局部、接口、因果变化、问答的完整逐件带声课程 | incomplete | 172/172项有当前静态图文件；17项有独立动态带声核查稿，114源片。 **缺口/限界：**155项无独立带声动态片；17项仍未通过实际听审/连续主观视听，canonical完整逐件课程验收0/172。 |
| R03 34定制件逐件真实几何和完整讲解 | incomplete | 34组原STEP/STL/native CAD来源逐成员SHA复核；34缩略图、已有原生位置资料可读。 **缺口/限界：**独立CAD-01至CAD-34完整带声课程0/34；相关BOM镜头仅能作共享/间接素材。6项是地面工装，不能都装入飞行模型。 |
| R04 9系统完整关系与运行原理讲解 | incomplete | A1/A2/A3/A4有55个独立片源及4带声系统核查稿。 **缺口/限界：**A5/A6/A7/B1/C1缺独立系统带声动态课；4现有系统仍未主观验收，完整系统验收0/9。 |
| R05 P01–P08逐原理动态教学 | incomplete | 8个互动实验有实际行为记录，每个5状态，自动行为检查通过；既有审查打开过各实验选定状态。 **缺口/限界：**sourceAuditComplete=false、overallAccepted=false；没有8条canonical独立完整带声原理影片。开篇八课不可替代P01–P08。 |
| R06 逐步assembly视频与初学者能跟上的连接关系 | incomplete | 实际219.86秒原CAD逐组归位无声核查母片可读，17段为15组归位+intro/outro。 **缺口/限界：**无音轨、时间轴暂定、连续内容审查未通过；归位动画不能替代逐接口解释。旧母片及层级引用不可达；对应可编辑制作源尚未定位，不能说已确认某blend丢失。 |
| R07 原生几何身份、总装浏览和原位置读取 | proven | 本地原生vehicle.usdc、层级/名称来源表与集成浏览器记录存在；既有浏览记录载入655source nodes、688mesh identities。 **缺口/限界：**证明范围是原CAD三角化/源位置与浏览定位；未求解native mates，未认证制造、压力或飞行。 |
| R08 虚拟组装对齐、真实接口/配合检验 | incomplete | 部分选定件有原层级位置与教学装回/关系镜头，源中nativeMatesSolved=false。 **缺口/限界：**未找到覆盖全部172/34/9接口的配合约束求解、间隙/干涉/同轴/接触/数量版本QC验收矩阵。统一浏览缩放/平移不等于配合验证。 |
| R09 每环节教学质量检查 | incomplete | 21现有核查稿有当前SHA对应的离散画面和正常速度技术播放记录；来源特征、句/动作、声音保持等门已制定。 **缺口/限界：**21实际听审和连续主观内容审查pending；其余完整课程/装配环节无逐环节通过记录。技术播放、双ASR和SHA不等于听懂或内容正确。 |
| R10 全部接口实物/工程QC | missing | 本次审查范围内只有来源、教学及软件/媒体QA证据。 **缺口/限界：**没有本次新造硬件逐接口尺寸/公差/密封/承载/可靠性/计量校准验收记录，不能把教学图或CAD可视化当QC证书。 |
| R11 仿真平台实际试用与原案例执行 | proven | 原输入HalfCatSim1.3.8由LibreOffice原生重算24.23秒；官方OpenRocket24.12实际执行原有1案例，872点，抵达ground event。 **缺口/限界：**此proven只指已有运行日志与不改输入的执行；存在回收高速警告，不能解释为物理/结构/全系统认证。 |
| R12 由仿真证明本次完整复现真实有效 | incomplete | 存在原案例重算和参数式飞行模拟执行证据。 **缺口/限界：**没有CAD应力/压力/热/配合的完整校核或实测对照闭环；表格L858与独立ORK/ENG的L1018非同基线已成立的证据。RASAeroII未执行。 |
| R13 原作者真实试验/飞行史证据 | indirect | 原指南3.2列19次地面试验，3.3列18条发射标题（后2条SN02）；官方出版物/版本/照片及已知失败/修订已有可追溯索引。 **缺口/限界：**这些是设计家族的原作者历史证据，不是本次虚拟复现或新实物验收；配置不同，未取得对应原始DAQ/遥测、校准数据和完整连续作者视频。 |
| R14 本次复现/新硬件真实有效的直接证据 | missing | 未发现本次项目独立实物制造、地面测试或飞行测量记录。 **缺口/限界：**原作者历史、仿真结果、原生CAD、媒体QA均不能代替本次实物检验和版本一致性证明。 |
| R15 完整可下载、可编辑、可恢复交付 | incomplete | 已发布12实际归档共4213722653bytes；repo截止快照4包fresh通过，本轮补最后小包108成员及legacy154成员收据后共6包；同一merged根现已有1077成员逐SHA记录。 **缺口/限界：**其余6大包fresh验证pending；同一干净位置按层覆盖的完整工程恢复/运行pending。A1-04单文件重开不等于全工程。 |
| R16 当前21片真实存在与技术播放 | proven | 本审计重新读取21实际媒体并流式计算SHA、ffprobe；与当前ledger SHA逐条比对。技术正常速度播放证据文件可核。 **缺口/限界：**本次没有新播放/解码/听审；读取既有技术报告不能算新的人类内容验收，21片始终工作核查稿。 |

## 当前实际数量

- 172物料、34定制件、9系统、8原理，canonical226场景；计划1156子镜。静态物料图文件覆盖172/172。
- 实际带声工作稿21：17物料+4系统，按实际视频帧数/帧率合计1901.125000秒（31分41.125秒）。源片169，当前存在169，逐SHA与ledger一致169。
- 完整验收：物料0/172、定制件0/34、系统0/9、原理0/8。21工作稿不可计成canonical完成。
- 34组STEP/STL/SLDPRT按原ZIP成员实际读取并比对SHA；共享BOM课不能重复计成34定制课。
- 8互动原理有行为稿；8开篇课是另一套引导片，不能抵作P01–P08完整独立原理讲解。
- 12已上传归档共4,213,722,653bytes；repo快照4包fresh通过，本轮另核最终小包108成员及legacy154成员收据，当前6包，另6大包及完整合并恢复pending。
- 同一merged根本轮读到3份归档成员恢复收据、合计1077条SHA记录（其中core815+legacy154+tiny108）。只是局部合并，整体应用重开/播放仍pending。
- 单件USD实际25/34；9项从来没有独立USD的已有缺口不冒充原ZIP丢失，原STEP/STL/native成员均在。

## 21个工作核查稿：当前实际文件与SHA

| 条目 | 秒 | 当前媒体SHA256 | 路径 |
|---|---:|---|---|
| A1-01 | 48.208333 | `18ae9c9f7502c7975d30ca39ffa70e0f5715733fed038a677fdfcfadcbde1dc3` | `outputs/rocket-v2/逐件动态样章/A1-01/A1-01_逐件中文动态样章_核查稿.mp4` |
| A1-16 | 52.458333 | `6f3fb66637f0265290d4c6ddcddbc4f35200fabcc17d533eb60e1907ee08d93f` | `outputs/rocket-v2/逐件动态样章/A1-16/A1-16_逐件中文动态样章_核查稿.mp4` |
| A3-12 | 47.458333 | `05eafdb34fc1a4afe698b6c5480ccaa3b5acf8137577aa198f27eadcdf8ffbf0` | `outputs/rocket-v2/逐件动态样章/A3-12/A3-12_逐件中文动态样章_核查稿.mp4` |
| A1-05 | 57.375000 | `a8e242f956682228a93b7e06a96217f13e39c4b35327e9e2db2083c71c801b8c` | `outputs/rocket-v2/逐件动态样章/A1-05/A1-05_逐件中文动态样章_核查稿.mp4` |
| A1-13 | 83.916667 | `11d8c51eff501896f68f3e164be851da2da4025fb7b380aa497b5904b363eb4a` | `outputs/rocket-v2/逐件动态样章/A1-13/A1-13_逐件中文动态样章_核查稿.mp4` |
| A1-02 | 66.833333 | `e25f8d7aa0a34ed79f50fcce7a668f8cda51252240f764a2e8079c015ae220a3` | `outputs/rocket-v2/逐件动态样章/A1-02/A1-02_逐件中文动态样章_核查稿.mp4` |
| A1-03 | 69.541667 | `e80724a963a1b2d6d9a8bcef9b6f30e6d543f65aa711c80e83ab4ff29d7d5b27` | `outputs/rocket-v2/逐件动态样章/A1-03/A1-03_逐件中文动态样章_核查稿.mp4` |
| A1-04 | 69.000000 | `8d0ec030ef24ebbbd768db0cd524d6cc7808da8bc0e36191bcea535d0cfdc724` | `outputs/rocket-v2/逐件动态样章/A1-04/A1-04_逐件中文动态样章_核查稿.mp4` |
| A1-14 | 97.125000 | `95711f5c84644b99fbcfe4805aa054255df7180601dfbcb8688f2933ac839023` | `outputs/rocket-v2/逐件动态样章/A1-14/A1-14_逐件中文动态样章_核查稿.mp4` |
| A1-15 | 101.708333 | `a21c4a58599f5bc68f842036d4eef07ceb67aad249c925c93a33a3c65bfd89e9` | `outputs/rocket-v2/逐件动态样章/A1-15/A1-15_逐件中文动态样章_核查稿.mp4` |
| A1-06 | 83.875000 | `38e32240e55f813b3d3b565fdc1b9049f1998cbac2384902dc8e700efb7835b4` | `outputs/rocket-v2/逐件动态样章/A1-06/A1-06_逐件中文动态样章_核查稿.mp4` |
| A1-07 | 83.958333 | `f0d39fc4c8ef3a800d6e2dc2485d140d615e9bfd77859e52b656066edb0e53e6` | `outputs/rocket-v2/逐件动态样章/A1-07/A1-07_逐件中文动态样章_核查稿.mp4` |
| A1-12 | 77.458333 | `0b14ad7a8c5c5d277bcc3bfa68ebaea69f20a40edb635482e81201084902e56b` | `outputs/rocket-v2/逐件动态样章/A1-12/A1-12_逐件中文动态样章_核查稿.mp4` |
| A1-08 | 80.708333 | `dcd4ed987f4f96adf206f825872eb48f72f14e591d97ceecb4620faf3e34fe27` | `outputs/rocket-v2/逐件动态样章/A1-08/A1-08_逐件中文动态样章_核查稿.mp4` |
| A1-09 | 74.625000 | `afd3ffbc35fd5deb4d735002a0369297c0c581dd2f484c17768793a0e436fba0` | `outputs/rocket-v2/逐件动态样章/A1-09/A1-09_逐件中文动态样章_核查稿.mp4` |
| A1-10 | 94.000000 | `c111bfee21c143b7ecab30203d59a90ed11d58b22ddeb24c42b0fb5dd4d66ae3` | `outputs/rocket-v2/逐件动态样章/A1-10/A1-10_逐件中文动态样章_核查稿.mp4` |
| A1-11 | 83.250000 | `169509b116c5e1a7e93e67a451b7f0dc3d20eda68402708eaf7ff3cf9afa5b28` | `outputs/rocket-v2/逐件动态样章/A1-11/A1-11_逐件中文动态样章_核查稿.mp4` |
| SYS-A3 | 85.041667 | `8462a6659be40c9d378c4f88f96d5e018aa030c2caf1745127ae718f855e6b4a` | `outputs/rocket-v2/系统动态样章/A3/A3_系统中文动态样章_核查稿.mp4` |
| SYS-A1 | 144.791667 | `108991f3e4111bd6a694bd34443076c1877bf605f0aa377024037d260fe08a3c` | `outputs/rocket-v2/系统动态样章/A1/A1_系统中文动态样章_核查稿.mp4` |
| SYS-A4 | 151.000000 | `6c6bf60c5e9129d8bbecba11b493ce07e21bcb4814f2e9614b39d5a27d82d106` | `outputs/rocket-v2/系统动态样章/A4/A4_系统中文动态样章_核查稿.mp4` |
| SYS-A2 | 248.791667 | `302b78ffb2fecf71c9edf9d782a005e7fd9aef88c0a2e5b1e25f8a39b31b1a7e` | `outputs/rocket-v2/系统动态样章/A2/A2_系统中文动态样章_核查稿.mp4` |

所有上述片的实际听审与连续主观内容验收仍pending；历史技术播放记录不被本审计升级为内容通过。

## 缺失独立完整动态课程清单

- 物料155项：A1-17, A1-18, A1-19, A2-01, A2-02, A2-03, A2-04, A2-05, A2-06, A2-07, A2-08, A2-09, A2-10, A2-11, A2-12, A2-13, A2-14, A2-15, A2-16, A2-17, A2-18, A2-19, A2-20, A3-01, A3-02, A3-03, A3-04, A3-05, A3-06, A3-07, A3-08, A3-09, A3-10, A3-11, A3-13, A3-14, A3-15, A4-01, A4-02, A4-03, A4-04, A4-05, A4-06, A4-07, A4-08, A4-09, A4-10, A4-11, A4-12, A4-13, A4-14, A4-15, A4-16, A4-17, A4-18, A4-19, A4-20, A4-21, A5-01, A5-02, A5-03, A5-04, A5-05, A5-06, A5-07, A5-08, A6-01, A6-02, A6-03, A6-04, A6-05, A6-06, A6-07, A6-08, A6-09, A6-10, A6-11, A6-12, A6-13, A6-14, A6-15, A6-16, A6-17, A6-18, A6-19, A6-20, A6-21, A6-22, A6-23, A6-24, A6-25, A6-26, A6-27, A7-01, A7-02, A7-03, A7-04, A7-05, A7-06, A7-07, A7-08, A7-09, A7-10, A7-11, A7-12, A7-13, A7-14, A7-15, A7-16, A7-17, A7-18, B1-01, B1-02, B1-03, B1-04, B1-05, B1-06, B1-07, C1-01, C1-02, C1-03, C1-04, C1-05, C1-06, C1-07, C1-08, C1-09, C1-10, C1-11, C1-12, C1-13, C1-14, C1-15, C1-16, C1-17, C1-18, C1-19, C1-20, C1-21, C1-22, C1-23, C1-24, C1-25, C1-26, C1-27, C1-28, C1-29, C1-30, C1-31, C1-32, C1-33, C1-34, C1-35, C1-36, C1-37。
- 定制件34项：CAD-01, CAD-02, CAD-03, CAD-04, CAD-05, CAD-06, CAD-07, CAD-08, CAD-09, CAD-10, CAD-11, CAD-12, CAD-13, CAD-14, CAD-15, CAD-16, CAD-17, CAD-18, CAD-19, CAD-20, CAD-21, CAD-22, CAD-23, CAD-24, CAD-25, CAD-26, CAD-27, CAD-28, CAD-29, CAD-30, CAD-31, CAD-32, CAD-33, CAD-34。
- 系统5项：A5, A6, A7, B1, C1。
- canonical原理8项：P01, P02, P03, P04, P05, P06, P07, P08。

JSON逐项表包含172+34+9+8条的图/源/接口/动态课状态与SHA；`currentPilots`保存全部169源片、当前媒体及技术报告的复核结果。

## assembly、对齐与QC

归位母片：`outputs/rocket-v2/assembly-review/原CAD逐组归位_无声核查母片.mp4`；SHA `19f66326f8c707d0d73bc03a6054b5f1c551c8234b44a71e717cbe900a1b06ca`，实际219.866667秒，17段＝15组+片头片尾，无声、未验收。
原母片引用路径 `${SIBLING_WORKSPACE_ROOT}/new-chat/work/assembly-film/silent-master.mp4` 当前不存在；旧source hierarchy路径也不可达。该记录未声明blend路径；只能说对应可编辑制作源尚未定位，不能宣称某已知blend丢失。项目和公开包清单有母片、时间轴、计划、原生vehicle/hierarchy，详见同目录`assembly-source-portability-gap.json/md`；它们不能自动替代母片编辑源。
原生浏览已支持身份/源位置读取；`nativeMatesSolved=false`、`manufacturingValidated=false`、`flightValidated=false`。未找到覆盖全物料/定制件/系统的配合求解、干涉、同轴、接触、数量和版本逐接口验收矩阵。
QC应分为教学内容/媒体技术与几何工程/实物验证。前者已有21片部分证据；后者不能由看起来对齐、教学颜色、解码或ASR推断。

## 仿真与真实有效性的证据层级

HalfCatSim原案例确实经LibreOffice原生重算；原298072公式的122062个#N/A位置/类型相同，已有终止分支解释，不是122062次独立求解失败，也不是所有活动计算/物理均已验证。
官方OpenRocket24.12确实执行原案例1次、872点、ground event，无错误/abort；保留回收高速警告。原输入未改，但这是参数式模型案例执行，不是CAD强度/压力/制造或新实物认证。RASAeroII未执行。
表格L858与独立ORK/ENG的L1018尚未建立同一基线。旧仿真索引同时有pending字段和后写actual execution，不应只摘旧字段否认已运行。
原作者指南确列19次地面试验和18条发射史（后2条SN02），可证明设计家族并非纯CAD概念，且有失败和已知修订。配置不同、原始DAQ/遥测/校准和完整连续视频缺失；不证明本次复现或新造实物真实有效。

## 本次复核的核心文件SHA

| 文件 | SHA256 |
|---|---|
| `work/rocket/parts.json` | `a74bae8de34cc70c6975813aad74c97a90883ee5698cee62bdb6d350c3c6bf20` |
| `work/rocket/custom-parts.json` | `1c793f9521e17a79cf1d38e2da6864dbaebc350dfd7a060fc1d94435376f5510` |
| `work/rocket/groups.json` | `59a0fbbed5effffa5ab17c0bda4edcb11912d5d8a2f5565e5d840335eb72b300` |
| `work/rocket/principles.json` | `3c93495d51ed696c1e7db155cd78e10759023f62d55a84c53e1e537049bd8d90` |
| `work/rocket/scenes.json` | `ba8dfe0e9d23b0f8c7a08177d447b748eb88691faa5943c13a4597db5dd92282` |
| `work/rocket-v2/full-course-production/curriculum.json` | `cdb67110103f916f1d6170305f8068c1aa95f2140032d6a1a7d6149d47efafc5` |
| `work/rocket-v2/full-course-production/coverage.json` | `cf10d6d7b38643624b976a447304363b8381977467e971dd355bbe9972b1feb0` |
| `work/rocket-v2/full-course-production/production-ledger.json` | `8096c8e9ccbd3d42e96f7b8d4b435bdbff24d38398945a06c23c8060b7784c65` |
| `work/rocket-v2/full-course-production/full-coverage-quality-gates.json` | `cafd840eabac8bfef93f7f6274baa9477ff9aba26baa5c562191301f2fd66057` |
| `work/rocket-v2/full-course-production/custom-groups-asset-audit.json` | `3fdf2ae25cb280981702333752f928253c52388455c6e4a0d7db3cece253b2de` |
| `work/rocket-deadline-publish/repo/README.md` | `1039d808832fa2b108d075fe40b21e293cacf8d920bd77bd447c9f274ad9a2f3` |
| `work/rocket-deadline-publish/repo/AI_HANDOFF.md` | `a72ce26abf3ac6f940dbf8ee3236e556ca98720c4405d1f4da5806242d54f294` |
| `work/rocket-deadline-publish/repo/RESTORE.md` | `1ace41a66406bec8958d791b48ff5198cef44aecf9d4db45d8613df41dc0b1d9` |
| `work/rocket-deadline-publish/repo/RELEASE_ASSETS.json` | `44651cb5c4684c04caa0774fd3457468106116387241c8ea3685c906c9be3de2` |
| `work/rocket-deadline-publish/repo/state/stage.json` | `fb3b6c664a847ee2afd5a2c2f4acb227fc9c200483de626b89b9e367554fc34f` |
| `work/rocket-deadline-publish/repo/state/checkpoint.json` | `42327c72e778bd617d6891e71089f4e5daf05cc2abab4451a92c31ad57e3aa50` |
| `work/rocket-deadline-publish/repo/state/backlog.json` | `9f7b18e055ba3a3dfeb52ac4e31559c0cd0024c78639c0ea531bd8f7d7cc45cd` |
| `outputs/rocket-v2/assembly-review/原CAD逐组归位_无声核查母片.mp4` | `19f66326f8c707d0d73bc03a6054b5f1c551c8234b44a71e717cbe900a1b06ca` |
| `work/rocket-v2/qa/native-integrated-browser-review.json` | `3e7c9a30195dff1c7f58baa68ef0d787bccd1c53fb28875471c16a32c7f75ac2` |
| `work/rocket-v2/principles-dynamic-qa.json` | `5fa598d8b8a3566b68e18eafd0211ea21f6583d76807125100c2fcf44aeee322` |
| `work/rocket-v2/qa/external-evidence/evidence-register.json` | `fec5c47b958d2486575c615388ddfc6b6c5cb0f15b9a953a8fefe833daed1335` |
| `work/rocket-v2/qa/external-evidence/official-existing-simulation-result.json` | `c180a46fb7d93b0b2ea307d1f7cc2652681f6500941c3a2be066cbfa7d64ee46` |
| `work/rocket-v2/simulation/native-recalculation-result.json` | `05b0b5bc38313d7f2934b0e62fe1a3358b9e555c54b18811b9e4fac711c9dd05` |
| `work/rocket-deadline-publish/fresh-editable-reopen-proof/reopen-proof.json` | `6be834bb3a7f5eabcc240a5d29f8e55e3433e9b2538212d666cd146170b1ff6c` |

## 审计限界与保护

共核本地文件/ZIP成员863条；当前缺失或与旧SHA不符记录0条，详见JSON `fileIssues`。
另9个历史上未提供独立USD的可选路径明确列在`knownUnavailableOptionalIndividualUSD`，不把它们算成此次缺失/漂移。container duration合计1901.126664秒，因逐片毫秒舍入较帧数基准多约1.664ms。
没有把缺失的可重生PNG缓存说成仍在；历史QA JSON/SHA可保留，但不能冒称全部proof栅格都可重开。
当前repo只读：HEAD和working tree状态前后一致；canonical五JSON的SHA前后一致。写入范围仅本独立审计目录。
本审计不是完整课程验收、工程适用性认证或实际听审。
