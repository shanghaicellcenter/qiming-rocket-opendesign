# 逐组归位母片：已有制作源恢复路径核查

**确证缺口是旧引用不可达，对应可编辑制作源尚未定位；不是已经证明某个已知blend丢失。**

- 声明文件 `${WORKSPACE_ROOT}/outputs/rocket-v2/assembly-review/接入与核查状态.json`，字段 `source`：`${SIBLING_WORKSPACE_ROOT}/new-chat/work/assembly-film/silent-master.mp4` 当前不存在。类型：silent rendered MP4, not editable blend。
- 声明文件 `${WORKSPACE_ROOT}/work/rocket-v2/assembly-sequence.json`，字段 `sourceHierarchy`：`${SIBLING_WORKSPACE_ROOT}/new-chat/work/native-cad/vehicle.hierarchy.json` 当前不存在。类型：native hierarchy JSON; local replacement exists but reference was not rewritten。

本项目仍保存母片、时间轴、原生vehicle及层级；没有改写任何引用。

| 保留文件 | SHA256 |
|---|---|
| `${WORKSPACE_ROOT}/outputs/rocket-v2/assembly-review/原CAD逐组归位_无声核查母片.mp4` | `19f66326f8c707d0d73bc03a6054b5f1c551c8234b44a71e717cbe900a1b06ca` |
| `${WORKSPACE_ROOT}/outputs/rocket-v2/assembly-review/silent-timeline.json` | `d96a94b54bce0396c9581da0e22bbcba610fda72a92ef677a32d064bf44aaf89` |
| `${WORKSPACE_ROOT}/outputs/rocket/source-inputs/partner-cad/native-cad/vehicle.usdc` | `93be117e7bdd28f2ccba30a532f8c9eb728fdf0857d63e8d12c24dd4b21d1d58` |
| `${WORKSPACE_ROOT}/outputs/rocket/source-inputs/partner-cad/native-cad/vehicle.hierarchy.json` | `73b81ad82022a9ac421e27468fe1bec59e6c95538d96df1f0bd8d6cc29a1732f` |
| `${WORKSPACE_ROOT}/work/rocket-v2/assembly-sequence.json` | `0df8bf94f5135e63cb166da2b9471646e2395c49b667547f9da6095c0738ae4a` |
| `${WORKSPACE_ROOT}/work/rocket-v2/assembly-previs-plan.md` | `107238672aa46da03c454188a40fb854a652f4793afadc3ca33f287a9699d5ef` |

## 12个公开包的清单证据

| 成员 | 所在最终包 | SHA256 |
|---|---|---|
| `outputs/rocket-v2/assembly-review/silent-timeline.json` | `qiming-production-source-voice-01-v2.tar.gz` | `d96a94b54bce0396c9581da0e22bbcba610fda72a92ef677a32d064bf44aaf89` |
| `outputs/rocket-v2/assembly-review/原CAD逐组归位_无声核查母片.mp4` | `qiming-priority-native-media-interactive-01-of-02.tar.gz` | `19f66326f8c707d0d73bc03a6054b5f1c551c8234b44a71e717cbe900a1b06ca` |
| `outputs/rocket-v2/assembly-review/接入与核查状态.json` | `qiming-production-source-voice-01-v2.tar.gz` | `7f4d649217596a8c576029ffb9d2335f14af9436f3dd2b79573169e2aeb53b7b` |
| `outputs/rocket/source-inputs/partner-cad/native-cad/vehicle.hierarchy.json` | `qiming-production-source-voice-01-v2.tar.gz` | `407dfc9cd034d33be3fdada1da0fb6a151ff5b42f866a56e991bc9dc3dde02b8` |
| `outputs/rocket/source-inputs/partner-cad/native-cad/vehicle.name-source-map.json` | `qiming-production-source-voice-01-v2.tar.gz` | `16cde67cf71de76e083026064aa068ed02b0fd6d9126336c300f675514e6effd` |
| `outputs/rocket/source-inputs/partner-cad/native-cad/vehicle.usdc` | `qiming-priority-native-media-interactive-01-of-02.tar.gz` | `93be117e7bdd28f2ccba30a532f8c9eb728fdf0857d63e8d12c24dd4b21d1d58` |
| `work/rocket-v2/assembly-previs-plan.md` | `qiming-production-source-voice-01-v2.tar.gz` | `107238672aa46da03c454188a40fb854a652f4793afadc3ca33f287a9699d5ef` |
| `work/rocket-v2/assembly-sequence.json` | `qiming-production-source-voice-01-v2.tar.gz` | `5f7865dcfdf269413fff5ad618c7839f707a7ae1b177e67d0c010eb4012cfeb9` |
| `work/rocket-v2/native-selected.blend` | `qiming-priority-editable-sources-03-of-03.tar.gz` | `a233468c7da0838e44987c0a0b06d4c77440e5a636efe4445a3f3b22bc8e6a7b` |

已读finalWinnerTable的6336路径、95个blend文件名；assembly-film/silent-master及明确assembly blend命名匹配0。该检索不是逐blend场景重开，不证明其他未标识文件一定不含有关源。

root可向已获授权的Anatomy/partner chat索取已有逐组归位编辑源、生成脚本/scene映射及旧工程或公共恢复入口；本轮不新建动画/重建母片。

此报告仅恢复核查，无新生产、下载、Blender或远端任务。
