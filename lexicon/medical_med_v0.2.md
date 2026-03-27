# LoongEnglish 第一份词表：医系 v0.2

这是 `LoongEnglish` 的第一份词表，围绕“医”这一核心概念展开。

这一版修正了 v0.1 的一个关键问题：

**“医”不再使用拼音词根 `yi`，而改用从现有英语中抽出来的真实医学词根 `med`。**

这样做的目的，是让 `LoongEnglish` 既保留中文式组合能力，又不完全脱离现有英语材料。也就是说，我们不是凭空发明一个新音节，而是从英语已经存在的 `medical / medicine / med` 这一组词里抽取出一个稳定词根，再按中文的构词方式重组。

## 造词原则

### 1. 主词根来自现有英语

- `med` = 医

这里选用 `med`，原因有三点：

- 它直接来自现有英语里的 `medical` / `medicine`
- 它足够短，适合大规模组合
- 它已经天然带有医学领域识别度

因此，后续医系词优先围绕 `med` 展开，而不再使用 `yi` 这类拼音词根。

### 2. 保持中文组合顺序不变

中文是前项修饰后项，所以这里统一采用：

- `医 + X` -> `med-X`
- `医 + X + Y` -> `med-X-Y`

不倒装，不追随原英语现成搭配，只保留中文本来的组合次序。

### 3. 后项使用基础英语词

后项优先使用短、稳、透明的基础英语词，例如：

- `person`
- `house`
- `skill`
- `study`
- `drug`
- `care`
- `check`
- `case`
- `cover`
- `book`
- `field`
- `tools`
- `system`

### 4. 优先保留词族感

现有英语的一个问题是：医学领域里的高频词并不共形。

例如：

- `doctor`
- `hospital`
- `medicine`
- `treatment`

它们都属于同一语义场，但字形上并没有明显家族关系。

而在 `LoongEnglish` 里，我们希望：

- `医生`、`医院`、`医术`、`医学`、`医疗`

这些词在形态上也显式属于同一词族，因此统一挂在 `med-` 下面。

## 医系词表

| 中文词 | 原英语 | LoongEnglish 新词 | 组合拆解 | 说明 |
| --- | --- | --- | --- | --- |
| 医 | medicine / medical | `med` | 医 | 医疗语义总词根 |
| 医生 | doctor | `med-person` | 医 + 生 | 基础职业词，突出同根性 |
| 医师 | physician | `med-master` | 医 + 师 | 更正式、更专业的职业称谓 |
| 医院 | hospital | `med-house` | 医 + 院 | 机构或场所类统一挂在 `house` 上 |
| 医术 | medical skill | `med-skill` | 医 + 术 | 强调技术、能力、手艺 |
| 医学 | medicine / medical science | `med-study` | 医 + 学 | 学科类统一用 `study` |
| 医药 | medicine and drugs / pharmaceutical | `med-drug` | 医 + 药 | 偏药品与药物体系 |
| 医疗 | medical care / treatment | `med-care` | 医 + 疗 | 偏服务、照护、治疗过程 |
| 医治 | treat / cure | `med-treat` | 医 + 治 | 动词型表达 |
| 医护 | medical and nursing care | `med-guard` | 医 + 护 | 护按守护、照护处理 |
| 医案 | medical case | `med-case` | 医 + 案 | 病例、案例、档案体系 |
| 医检 | medical test / examination | `med-check` | 医 + 检 | 检查、检验类表达 |
| 医保 | medical insurance / healthcare coverage | `med-cover` | 医 + 保 | 保按保障、覆盖处理 |
| 医保卡 | health insurance card | `med-cover-card` | 医 + 保 + 卡 | 三段组合示例 |
| 医书 | medical text / medical book | `med-book` | 医 + 书 | 文献、教材、读物类 |
| 医德 | medical ethics | `med-ethic` | 医 + 德 | 职业伦理类 |
| 医嘱 | doctor's orders / medical advice | `med-order` | 医 + 嘱 | 指令、处置说明类 |
| 医科 | medical field / medical department | `med-field` | 医 + 科 | 学科、科别、分科基元 |
| 医学院 | medical school | `med-study-house` | 医 + 学 + 院 | 完整保留中文顺序 |
| 医学生 | medical student | `med-study-person` | 医 + 学 + 生 | 学科加人的递归组合 |
| 医用 | medical-use / for medical use | `med-use` | 医 + 用 | 用途标签词 |
| 医用口罩 | medical mask | `med-use-mask` | 医 + 用 + 口罩 | 产品命名示例 |
| 医疗器械 | medical devices | `med-care-tools` | 医 + 疗 + 器械 | 设备类复合词 |
| 医疗系统 | healthcare system | `med-care-system` | 医 + 疗 + 系统 | 系统类复合词 |
| 医药费 | medical expenses | `med-drug-fee` | 医 + 药 + 费 | 费用类复合词 |

## 为什么不用 `yi`

`yi` 的问题不在于不能用，而在于它不符合这个项目更长远的方向。

如果一个核心词根完全脱离现有英语体系，那么它虽然保留了中文发音，但会削弱两件事：

- 与现有英语语料的连接
- 被非中文用户猜测和吸收的可能性

`med` 更合适，因为它同时满足三件事：

- 来自真实英语
- 可被中文式继续组合
- 一眼能看出和医学有关

所以这套词表现在遵循的新原则是：

**核心语义词根，优先从现有英语中抽取；组合顺序，优先保留中文结构。**

## 当前结论

这一版词表验证的是另一条更重要的规则：

**LoongEnglish 不是拼音英语，而是“英语词根 + 中文组合”的重构英语。**

因此这套写法里：

- `med-person`
- `med-house`
- `med-skill`
- `med-study`
- `med-care`
- `med-study-house`

它们既比现有英语更成体系，又比纯拼音方案更容易与原英语世界接轨。

## 下一步建议

下一轮可以继续往四个方向扩：

1. 做 `药` 系词表，例如 `药店 / 药方 / 药效 / 药量`
2. 做 `病` 系词表，例如 `病人 / 病房 / 病史 / 病程`
3. 做 `护` 系词表，例如 `护士 / 护理 / 护工 / 护具`
4. 做 `诊` 系词表，例如 `门诊 / 诊室 / 诊断 / 诊疗`

如果你要，我下一步可以直接继续把整套医学词表扩成 `100` 个词，并统一成“英语词根 + 中文组合”的规则体系。

