# 治理文件完整性检查 — 2026-08-17

> 检查者: ACE Runtime 云端兜底 (Keeper)
> 检查时间: 2026-08-17
> 检查范围: mine-seed 仓库 governance/ 目录及相关治理文件

## 检查结果: 通过

本次检查未发现治理文件异常缩减。所有 governance/ 下的 .md 文件行数正常。

## governance/ 目录文件行数

| 文件 | 行数 | 状态 |
|------|------|------|
| governance/GOVERNANCE.md | 36 | 正常 |
| governance/decisions/README.md | 11 | 正常 |

## 02_MEMORY/assets/governance/ 文件行数

| 文件 | 行数 | 状态 |
|------|------|------|
| GV-001-admission-engine.md | 51 | 正常 |
| GV-002-civilization-freeze.md | 49 | 正常 |
| GV-003-red-blue-round-table.md | 58 | 正常 |
| MEMORY_MCP_EVALUATION.md | 164 | 正常 |

## C-004 事故相关文件状态

2026-07-18 事故中涉及的文件：
- `governance/civilization_overview.md` — **未找到**（在 mine-seed 仓库中不存在）
- `governance/external_learning_protocol.md` — **未找到**（在 mine-seed 仓库中不存在）

**分析**: 这两个文件在当前 mine-seed 仓库（main 分支，depth=1 克隆）中不存在。可能原因：
1. 文件位于其他分支或已被迁移
2. 文件在事故后通过 git 历史恢复但后续被移动到其他位置
3. 文件位于用户本地未推送的版本中

**建议**: 下次巡检时确认这两个文件的实际位置。如已迁移，更新 C-004 防护规则中的文件路径引用。

## C-004 防护执行情况

- 本轮巡检未修改 governance/ 下的任何文件
- 未发生简化版覆盖事件
- 完整性检查通过

## 基线建立

本次为首次在 r1-continuity-backup 中记录治理文件行数基线。后续巡检将与此基线对比，缩减超过 20% 的文件将记录到 reports/security_issue_YYYYMMDD.md。
