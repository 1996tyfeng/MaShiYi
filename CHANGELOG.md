# Changelog

本文件记录 Project MaShiYi 的重要更新。

---

## v0.4.7 — 2026-07-03

### Day 7 / Day 8 时间归属修正

- 将凌晨 04:00 的 5ml、下午约 15:00 分三次喝下的 25ml，以及“自主排便后踩到脚上”的记录，从 Day 8（2026-07-03）修正至 Day 7（2026-07-02）。
- 更新 `data/milk.csv` 与 `data/health.csv`，Day 7 改为部分记录（`record_quality=partial`），不再标记为完全缺失。
- 新增 `diary/DAY_007.md`，记录长时间空腹、补奶和便便踩脚事件。
- 更新 `diary/DAY_008.md`，仅保留 2026-07-03 第一次主动尝试羊奶泡软奶糕的记录。

---

## v0.4.6 — 2026-07-03

### Day 8 第一次尝试离乳食

- 更新 `data/milk.csv`，补充 Day 8 凌晨 04:00 的 5ml、下午约 15:00 分三次喝下的 25ml，以及第一次尝试羊奶泡软奶糕的记录。
- 更新 `data/health.csv`，补充长时间空腹、补奶后精神良好、自主排便踩到脚上，以及首次舔食奶糕时短暂咳嗽两下的观察。
- 新增 `diary/DAY_008.md`，完整记录 Day 8 的奶量、便便现场和第一次主动尝试离乳食。
- 更新 `diary/ACHIEVEMENTS.md`，新增“第一次主动尝试离乳食”。

---

## v0.4.5 — 2026-07-03

### Day 7 数据缺失标记

- 更新 `data/milk.csv`，明确标记 Day 7（2026-07-02）奶量记录缺失，不做估算。
- 更新 `data/health.csv`，将 Day 7 日常状态标记为记录缺失。
- 在备注中加入 `record_quality=missing`，避免后续统计时把缺失数据误判为零摄入或异常状态。

---

## v0.4.4 — 2026-07-01

### Day 6 体重与幼猫放电期

- 更新 `data/weight.csv`，补充 Day 6 体重 370g。
- 更新 `data/health.csv`，补充 Day 6 体重与“到处抓抓碰碰、探索欲增强”的行为观察。
- 更新 `diary/DIARY.md`，新增 Day 6 日记，记录 370g、全天奶量约 80ml，以及今天格外调皮、进入幼猫玩耍与放电阶段。
- 更新 `diary/ACHIEVEMENTS.md`，新增“体重达到 370g”和“进入幼猫放电期”。

---

## v0.4.3 — 2026-07-01

### Day 6 奶量记录

- 更新 `data/milk.csv`，补充 Day 6 11:30、15:30、18:00、18:30、23:00 的喂奶记录。
- 更新 `data/health.csv`，补充 Day 6 全天已记录奶量约 80ml。
- 记录 18:00 喂 10ml 后，18:30 左右再次叫饿并补奶 10ml，继续观察是否形成主动少量多餐节奏。

---

## v0.4.2 — 2026-06-30

### Day 5 奶量与分心吃奶

- 更新 `data/milk.csv`，补充 Day 5 04:00、11:30、15:20、18:20、22:00 的喂奶记录。
- 更新 `data/health.csv`，补充 Day 5 全天奶量约 119.5ml，以及“吃一会、玩一会、再回来吃”的喂奶节奏观察。
- 更新 `diary/DIARY.md`，补充 Day 5 奶量、分餐式吃奶和建立“专心吃奶，吃完再玩”节奏的观察建议。

---

## v0.4.1 — 2026-07-01

### 时间轴二次校正

- 按妈妈确认，原本拆成 2026-06-26 与 2026-06-27 的内容实际都属于 2026-06-26。
- 合并 `Day 1（2026-06-26）` 内容：310g、321g、吸手补奶、舔手、嘬毛毯、航空箱自主排尿等记录统一归入 Day 1。
- 将后续成长记录整体前移一天：原 Day 3 内容调整为 Day 2，原 Day 4 内容调整为 Day 3，原 Day 5 内容调整为 Day 4，原 Day 6 内容调整为 Day 5。
- 同步修正 `diary/DIARY.md`、`diary/ACHIEVEMENTS.md`、`data/milk.csv`、`data/weight.csv`、`data/health.csv`、`LORE.md` 与 `PROJECT_BIBLE.md`。

---

## v0.4.0 — 2026-07-01

### 时间轴修正

- 将 Day 0 起始日期从 `2026-06-26` 修正为 `2026-06-25`。
- 按妈妈提供的表格，统一 Day 与日期对应关系：Day0=2026-06-25，Day1=2026-06-26，Day2=2026-06-27，Day3=2026-06-28，Day4=2026-06-29，Day5=2026-06-30，Day6=2026-07-01。
- 同步修正 `diary/DIARY.md`、`diary/ACHIEVEMENTS.md`、`data/milk.csv`、`data/weight.csv`、`data/health.csv`、`README.md`、`LORE.md`、`PROJECT_BIBLE.md`、`prompts/chatgpt.md` 与 `prompts/codex.md`。
- 更新 Day 计算规则为：`Day = 记录日期 - 2026-06-25`。

---

## v0.3.2 — 2026-07-02

### Day 6 斗篷事件

- 更新 `data/health.csv`，补充 Day 6 早上的自主排便与斗篷被蹭脏记录。
- 更新 `diary/DIARY.md`，新增 Day 6 阶段性日记，记录金黄色偏软便便、屁股尾巴被蹭脏，以及灰色绒斗篷只剩约三分之一干净部分。
- 更新 `diary/ACHIEVEMENTS.md`，新增“第一次屎糊斗篷事件”。
- 更新 `LORE.md`，补充灰色绒斗篷从安全感物品到奶猫期元老级小被子的背景。

---

## v0.3.1 — 2026-07-01

### Day 5 第一次兔子踢

- 更新 `diary/DIARY.md`，补充小十一抱着小布偶练习兔子踢的记录。
- 更新 `diary/ACHIEVEMENTS.md`，新增“第一次兔子踢”。
- 更新 `LORE.md`，补充小布偶成为小十一第一位玩耍陪练的背景。

---

## v0.3.0 — 2026-07-01

### 成长观察协议

- 新增 `OBSERVATION_PROTOCOL.md`，正式记录“小十一成长观察协议”。
- 更新 `README.md`，在仓库结构与更新原则中加入观察协议。
- 更新 `prompts/chatgpt.md`，明确 ChatGPT 不只是记录，也需要观察成长趋势并在需要时即时提醒妈妈。

---

## v0.2.9 — 2026-07-01

### Day 5 第一件专属小布偶

- 更新 `diary/DIARY.md`，补充 Day 5 小布偶互动记录。
- 更新 `diary/ACHIEVEMENTS.md`，新增“第一件专属小布偶”。
- 更新 `LORE.md`，补充小布偶从窝里的陪伴物变成专属玩具的背景。

---

> 📖 今天的小十一，又长大了一点点。
