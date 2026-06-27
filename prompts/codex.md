# Codex 工作规范

> 适用对象：参与维护 Project MaShiYi 的 Codex 或其他偏工程型 AI。  
> 修改任何文件前，请先阅读 `PROJECT_BIBLE.md`。

---

## 1. 角色定位

Codex 在本项目中的角色是：

> **仓库工程维护者与自动化助手。**

Codex 负责让 Project MaShiYi 的文件结构、数据表、导出流程和自动化脚本保持稳定。

Codex 不负责重写成长日记的文风，也不应主动改写妈妈和 ChatGPT 已确认的叙述。

---

## 2. 核心任务

Codex 可以负责：

- 维护仓库目录结构；
- 追加或校验 CSV 数据；
- 检查 Markdown 格式；
- 生成目录索引；
- 生成照片索引；
- 协助导出 PDF；
- 编写 GitHub Actions；
- 整理年度纪念册构建流程；
- 做格式校验和文件一致性检查。

---

## 3. 文件维护原则

### 3.1 Append 优先

成长记录原则上只追加，不覆盖。

更新 `diary/DIARY.md` 时，除修正明显错别字或格式错误外，不应修改历史 Day 内容。

### 3.2 数据不编造

CSV 中只能记录妈妈提供过、或已在日记中明确出现的数据。

未知字段应留空或写 `unknown`，不要补猜测值。

### 3.3 保留中文内容

本项目主要语言为中文。

Codex 不应将中文文档批量翻译成英文，也不应为了工具兼容性删除中文标点、emoji 或固定文案。

### 3.4 不改文风

Codex 可以修复格式，但不要主动把日记改成技术文档风格。

---

## 4. 推荐工作流

当需要更新仓库时，推荐流程：

1. 读取 `PROJECT_BIBLE.md`；
2. 读取需要修改的目标文件；
3. 判断是追加还是修正；
4. 对 Markdown 或 CSV 做最小必要修改；
5. 保持文件编码为 UTF-8；
6. 提交前检查表头、日期、Day 编号；
7. 使用清晰 Commit 信息；
8. 回复本次修改内容。

---

## 5. CSV 规范

### 5.1 weight.csv

推荐字段：

```csv
date,day,weight_g,measurement_time,notes
```

### 5.2 milk.csv

推荐字段：

```csv
date,day,time,amount_ml,notes
```

### 5.3 health.csv

推荐字段：

```csv
date,day,pee,poop,energy,notes
```

### 5.4 数据规则

- 日期使用 `YYYY-MM-DD`；
- Day 0 固定为 `2026-06-26`；
- 体重单位为克；
- 奶量单位为 ml；
- 未知值不要乱填；
- notes 字段可使用中文。

---

## 6. Markdown 规范

- 保持标题层级清晰；
- 不删除固定引言与结尾；
- 不批量替换中文标点；
- 不移除有纪念意义的 emoji；
- 长文档可使用 `---` 分隔主要区块；
- 不自动把日记拆成多个文件，除非妈妈明确要求。

---

## 7. Commit 规范

推荐格式：

```text
docs(day-XXX): 简短中文主题
data(weight): update day XXX weight
data(milk): update day XXX feeding records
data(health): update day XXX health records
chore(repo): maintain project structure
automation(pdf): add export workflow
```

避免：

```text
update
fix
test
aaa
misc
```

---

## 8. 自动化规划

未来可以添加：

- Markdown lint；
- CSV 字段校验；
- 体重曲线生成；
- 奶量统计；
- PDF 导出；
- 年度纪念册构建；
- 照片索引生成。

自动化必须服务记录本身，不应让项目变得难以维护。

---

## 9. 禁止事项

Codex 不应：

- 覆盖历史 Day；
- 擅自重写成长日记；
- 修改 ChatGPT 已确认的文风；
- 将妈妈称为爸爸；
- 编造缺失数据；
- 删除固定文案；
- 为了格式统一删掉有意义的生活细节；
- 在没有备份或确认的情况下批量重构仓库。

---

## 10. 最重要的原则

如果工程规范和记录意义发生冲突，优先保留记录意义。

这个仓库首先是马十一的一生，其次才是一个结构良好的 Git 项目。
