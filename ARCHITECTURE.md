# 元御 · 智能体安全治理架构 v0.1

六层 + 一横切，收拢智能体从身份到评测的治理闭环。

## 六层

| 层 | 名称 | 职责 | 关键问题 |
|---|------|------|---------|
| L0 | 元法则 | 全体系判据总源，推演先行的决策法则 | 谁拍板、按什么拍板 |
| L1 | 身份权限 | 智能体唯一身份、能力边界、最小授权 | 它是谁、能碰什么 |
| L2 | 准入与行为闸 | 输入输出双闸、行为级评测 | 放行什么、拦住什么 |
| L3 | 输出治理 | 结果校验、幻觉拦截、话术规范 | 说的可信吗 |
| L4 | 记忆与数据治理 | 记忆归属、数据边界、不出域 | 记了什么、传给谁 |
| L5 | 审计可追溯 | 过程留痕、哈希链台账、可回放 | 出事能查吗 |
| L6 | 评测认证 | 可验证与过程评测，达标线机验 | 凭什么信它 |

## 一横切

**红蓝对抗进化循环**横切全部六层：规则资产经每日对抗持续打磨，拦截率、误伤、弹药数三条硬指标机验达标（详见 [taiji-loop](https://github.com/tanbopiao/taiji-loop)）。

## 配套组件

- [wuji-chaos](https://github.com/tanbopiao/wuji-chaos) — 无极：大模型混沌观测
- [liangyi-gates](https://github.com/tanbopiao/liangyi-gates) — 两仪：红蓝校准网关
- [zhenzhi-ledger](https://github.com/tanbopiao/zhenzhi-ledger) — 真值：哈希链台账（L5）
- [xuangui-verdict](https://github.com/tanbopiao/xuangui-verdict) — 玄圭：裁决筛选（L2）
- [feifei-guard](https://github.com/tanbopiao/feifei-guard) — 朏朏：岗位模板包（L2/L3 落地形态）
