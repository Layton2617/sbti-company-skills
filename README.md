# sbti-company

**27 个嘴替给你的产品泼冷水。**

决策前 2 分钟，拿到一份"27 种读法"的评论区报告。比开焦点小组快 100 倍、比问朋友狠 10 倍、比花钱做用户访谈便宜 5000 倍。免费、本地、不会向老板汇报你的蠢 idea。

基于 2026 年 4 月 Bilibili [@蛆肉儿串儿](https://www.sbti.ai/en) 发起的 SBTI（Silly Big Personality Test）27 种自嘲人格。

> 想要正经的产品评审版？→ [mbti-company](https://github.com/Layton2617/mbti-company)（16 个 MBTI 同事开专业评审会）

---

## 安装

```bash
git clone https://github.com/Layton2617/sbti-company.git ~/.claude/skills/sbti-company
```

下次打开 Claude Code 自动识别。

## 用法

```
吐槽一下：我想做一个给留学生的 AI 求职 App，$29/月
```

或者

```
照妖镜：今天又把消息发错群了
```

或者分队围攻：

```
围攻：我该不该辞职去开咖啡店
```

或者单独追问：

```
@SHIT 你再狠一点
@DRUNK 这事你怎么看
```

## 输出示例

**议题**：留学生 AI 求职陪跑 App $29/月

```
### SHIT · 暴躁现实派
这 idea 就是坨——"简历优化" GPT 免费做，"内推匹配"你拿不到真数据。
砍两个，All-in "拒信复盘 + 下一步行动"，才是没人做的。

### MALO · 吗喽
这关难打。"AI 求职"是新手村最挤的副本，boss 是 LinkedIn + Simplify
联合团本，你一个人进去就是送。先吃药，别 All-in。

### ATM-er · 送钱者
$29/月的人其实不是留学生，是焦虑的家长——你方案里谁是被默认压榨的
那一方，想清楚没？

（共 26 人发言……）

## BOSS 拍板综合
- 💬 高赞：SHIT「三件事各自都有人做，All-in 拒信复盘才是没人做的」
- 🎯 真话：三合一不是产品，是拼盘。选 1 个垂直打穿。
- 🚪 下一步：先别做 App，周末出 landing page 测 waitlist。
```

## 5 个场景

| 场景 | 用途 | 触发关键词 |
|---|---|---|
| **roast**（默认） | 27 人轮番吐槽 | 吐槽 / 乱喷 / 锐评 |
| **mirror** | 照妖镜，27 人认领你此刻状态 | 照镜子 / 我是不是 / 破防 |
| **gang-up** | 自动分队围攻辩论 | 该不该 / 要不要 / 围攻 |
| **growth-hack** | 增长黑客评论区 | 增长 / 获客 / 留存 / CAC |
| **kill-feature** | 砍需求会 | 砍 / 下线 / 精简 |

## 27 个人格（5 模组 + 1 兜底 + 1 隐藏）

| 模组 | 人格 |
|---|---|
| **Self** 自我 | BOSS / THIN-K / IMSB / IMFW |
| **Emotional** 情感 | LOVE-R / MUM / THAN-K / ATM-er |
| **Attitude** 态度 | OH-NO / MONK / MALO / JOKE-R / WOC! / OJBK / SHIT / FUCK / HHHH |
| **Action** 行动 | GOGO / ZZZZ / POOR / DEAD / Dior-s |
| **Social** 社交 | SEXY / CTRL / FAKE / SOLO |
| **Hidden** 隐藏 | DRUNK |

- **HHHH** = 兜底人格（SBTI 官方"测不出就是它"）
- **DRUNK** = 隐藏人格，只在沉重议题（分手 / 裁员 / 中年 / 失业）接替 BOSS 主持

## 安全机制

内置三道熔断：

| 议题 | 处理 |
|---|---|
| 自杀 / 自残 / 想死 / 活不下去 | 停止 27 人环节，返回专业危机资源（988 / 北京 010-82951332 等） |
| 合同 / 诉讼 / 投资 / 用药 / 医疗诊断 | 整场熔断，建议走专业渠道 |
| 真实姓名 / 具名公司 / 具名品牌 | 自动脱敏为"前任 / 前公司 / 某品牌" |
| 受保护群体歧视（种族 / 性别 / 宗教 / 残障 / 性取向 / 地域） | Con 队禁用攻击型人格 + BOSS 加免责 |

## 结构

```
sbti-company/
├── SKILL.md            # 入口 + 触发规则
├── orchestrator.md     # 编排（5×6 批量 subagent 方案）
├── personas/           # 27 份人格卡（含禁忌字段防串味）
└── scenarios/          # 5 个场景
```

## 数据来源

- 27 人格名 + official line 取自 [sbti.ai/en](https://www.sbti.ai/en)（官方站）
- 人设、语言风格、金句 **全部原创**，未抄题库
- 参考 MIT 项目 [bingran-you/sbti-cli](https://github.com/bingran-you/sbti-cli) 的 15 维分组

## 何时选 SBTI 而不是 MBTI

- 要"扎心段子 / 毒舌吐槽 / 自嘲" → SBTI
- 要"结构化评审 / 可执行决策" → [MBTI](https://github.com/Layton2617/mbti-company)
- 两个都想要 → 先 MBTI 给定性，再 SBTI 给情绪出口

## License

MIT
