# Changelog

本文件记录 Project MaShiYi 的重要更新。

---

## v0.2.4 — 2026-06-29

### Day 2 / Day 3 记录补充

- 更新 `data/milk.csv`，补充 Day 3 凌晨与早上的喂奶记录。
- 更新 `data/health.csv`，补充 Day 2 自主排尿与 Day 3 叫声减少、经常打呼噜等健康观察。
- 更新 `diary/DIARY.md`，新增 Day 2 与 Day 3 的阶段性记录。
- 更新 `diary/ACHIEVEMENTS.md`，新增“第一次自主排尿”和“第一次经常打呼噜”。
- 更新 `LORE.md`，补充从公司回家、航空箱自主排尿、到家后更安心的背景记录。

### 已记录的重要时刻

- Day 2：从公司回家途中，约 23 点多在航空箱里自主排尿。
- Day 3：01:00 到家后喝奶约 17ml，未排尿。
- Day 3：07:20 左右刺激排尿后喝奶约 12～13ml。
- Day 3：叫声明显比前两天少，开始经常打呼噜。

---

## v0.2.3 — 2026-06-28

### Project Bible 同步

- 将 `PROJECT_BIBLE.md` 同步到当前仓库结构。
- 补充 `LORE.md`、`ACHIEVEMENTS.md`、`MEDICAL.md`、`photos/README.md`、`letters/README.md` 的职责说明。
- 同步北京时间（UTC+8）与 Day 自动计算规则。
- 同步 `data/milk.csv` 当前字段：`date,day,time,amount_ml,pee,poop,notes`。
- 明确体重、奶量和排泄可实时更新，日记在妈妈要求“更新今天日记”时汇总。
- 补充 Day 2 已知事实：饭后称重 321g。

---

## v0.2.2 — 2026-06-28

### 时间规则

- 在 `prompts/chatgpt.md` 中新增时间与 Day 编号规则。
- 在 `prompts/codex.md` 中新增北京时间（UTC+8）记录标准。
- 统一规定：所有日期、Day 编号、CSV 日期和 Diary 日期，以妈妈发送消息时的北京时间为准。
- 明确 Day 编号公式：`Day = 记录日期 - 2026-06-26`。
- 当日期和 Day 编号冲突时，以日期为准重新计算 Day。

---

## v0.2.1 — 2026-06-28

### 数据结构升级

- 升级 `data/milk.csv` 表头，从 `date,day,time,amount_ml,notes` 调整为 `date,day,time,amount_ml,pee,poop,notes`。
- 将每顿喂奶后的排尿、排便情况与该顿奶量关联记录。
- 对已有 Day 0 与 Day 1 喂奶记录补充 `pee` / `poop` 字段。
- 未明确记录的排泄情况使用 `unknown`，避免补写不确定数据。

---

## v0.2.0 — 2026-06-27

### 架构升级

- 新增 `LORE.md`，用于记录马十一的背景、名字由来、早期安全感与长期可补充设定。
- 明确文档分工：`PROJECT_BIBLE.md` 负责项目规则，`LORE.md` 负责马十一自己的故事背景。
- 更新 `README.md`，加入新的仓库结构与文档分工说明。

### 新增档案

- 新增 `diary/ACHIEVEMENTS.md`，记录小十一成长过程中的重要“第一次”。
- 新增 `diary/MEDICAL.md`，记录医疗、疫苗、驱虫、体检与重要健康观察。
- 新增 `photos/README.md`，建立照片与视频索引规范。
- 新增 `letters/README.md`，作为妈妈写给小十一的信件目录。

### 已收录成就

- 欢迎回家。
- 拥有名字：马十一。
- 第一次踩奶。
- 第一次在新家安心睡着。
- 第一次正式称重。
- 第一次主动睡到妈妈头边。
- 解锁“嘬毛毯”。
- 第一次清楚表达“我还没吃饱”。
- 第一次吃饱后舔妈妈的手。

---

## v0.1.0 — 2026-06-27

### 初始化

- 建立 Project MaShiYi 仓库基础内容。
- 确认仓库用于长期维护《马十一》成长档案。
- 明确项目原则：真实记录、长期追加、数据与故事并重。

### 文档

- 扩展 `PROJECT_BIBLE.md` 为正式项目规范。
- 重写 `README.md`，作为仓库首页与项目封面。
- 重写 `diary/DIARY.md`，整理 Day 0 与 Day 1 的成长记录。

### 数据

- 规范化 `data/weight.csv`。
- 扩展 `data/milk.csv`，记录 Day 0 与 Day 1 的每顿奶量。
- 规范化 `data/health.csv`，记录排尿、排便与精神状态。

### 已记录的重要时刻

- Day 0：欢迎回家，小十一。
- Day 0：第一次裹着妈妈的灰色绒斗篷踩奶睡着。
- Day 1：第一次正式称重，310g（饭后）。
- Day 1：第一次主动爬到妈妈头边睡觉。
- Day 1：通过疯狂吸手表达“我还没吃饱”。
- Day 1：补奶后开始舔妈妈的手。
- Day 1：学会嘬毛毯进行自我安抚。

---

> 📖 今天的小十一，又长大了一点点。
