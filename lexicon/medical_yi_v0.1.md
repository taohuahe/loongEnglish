# LoongEnglish 第一份词表：医系 v0.1

这是 `LoongEnglish` 的第一份词表，围绕汉语词根 `医` 展开。

这份词表的目标，不是去复述现成英语，而是先建立一套**共享词根 + 可递归组合**的中式英语词族。也就是说，`医生 / 医院 / 医术 / 医学 / 医药 / 医疗` 这些在中文里同根的词，在新体系里也要保持同根，而不是像现有英语那样分散成 `doctor / hospital / medicine / treatment` 这种彼此断裂的词形。

## 造词规则

### 1. 固定主词根

- `yi` = `医`

这里先把 `yi` 设为医疗语义的统一主词根。后续所有医系词，优先围绕 `yi` 展开。

### 2. 保持中文组合顺序

中文是前项修饰后项，所以这里统一采用：

- `医 + X` -> `yi-X`
- `医 + X + Y` -> `yi-X-Y`

不倒装，不追现有英语词源，只保留中文组合逻辑。

### 3. 后项尽量用基础词

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
- `tool`
- `system`

### 4. 现代语义优先

有些汉字在现代词语里的作用，不按古义硬拆，而按现代组合功能处理。

例如：

- `医生` 里的 `生`，这里按“从业者 / 人”处理，所以记作 `person`
- `医院` 里的 `院`，这里按“机构 / 场所”处理，所以记作 `house`

## 医系词表

| 中文词 | 原英语 | LoongEnglish 新词 | 组合拆解 | 说明 |
| --- | --- | --- | --- | --- |
| 医 | medicine / medical / heal | `yi` | 医 | 医疗语义总词根 |
| 医生 | doctor | `yi-person` | 医 + 生 | 同根词族的基础职业词 |
| 医师 | physician | `yi-master` | 医 + 师 | 比 `yi-person` 更偏专业称谓 |
| 医院 | hospital | `yi-house` | 医 + 院 | 统一用场所词承接机构语义 |
| 医术 | medical skill | `yi-skill` | 医 + 术 | 强调技术、手艺、能力 |
| 医学 | medicine / medical science | `yi-study` | 医 + 学 | 学科类统一用 `study` |
| 医药 | medicine and drugs / pharmaceutical | `yi-drug` | 医 + 药 | 偏药物与药品体系 |
| 医疗 | medical care / treatment | `yi-care` | 医 + 疗 | 偏服务、照护与治疗过程 |
| 医治 | treat / cure | `yi-treat` | 医 + 治 | 动词型表达 |
| 医护 | medical and nursing care | `yi-guard` | 医 + 护 | 护按守护、照护处理 |
| 医案 | medical case | `yi-case` | 医 + 案 | 适合病例、案例、档案体系 |
| 医检 | medical test / examination | `yi-check` | 医 + 检 | 检查、检验统一用 `check` |
| 医保 | medical insurance / healthcare coverage | `yi-cover` | 医 + 保 | 保按保障、覆盖处理 |
| 医保卡 | health insurance card | `yi-cover-card` | 医 + 保 + 卡 | 三段组合示例之一 |
| 医书 | medical text / medical book | `yi-book` | 医 + 书 | 文献、教材、读物类 |
| 医德 | medical ethics | `yi-ethic` | 医 + 德 | 职业伦理类 |
| 医嘱 | doctor's orders / medical advice | `yi-order` | 医 + 嘱 | 指令、医嘱、处置说明 |
| 医科 | medical field / medical department | `yi-field` | 医 + 科 | 学科、科别、分科基元 |
| 医学院 | medical school | `yi-study-house` | 医 + 学 + 院 | 组合顺序完整保留 |
| 医学生 | medical student | `yi-study-person` | 医 + 学 + 生 | 学科 + 人 的递归组合 |
| 医用 | medical-use / for medical use | `yi-use` | 医 + 用 | 用途标签词 |
| 医用口罩 | medical mask | `yi-use-mask` | 医 + 用 + 口罩 | 产品命名示例 |
| 医疗器械 | medical devices | `yi-care-tools` | 医 + 疗 + 器械 | 设备类复合词 |
| 医疗系统 | healthcare system | `yi-care-system` | 医 + 疗 + 系统 | 系统类复合词 |
| 医药费 | medical expenses | `yi-drug-fee` | 医 + 药 + 费 | 费用类复合词 |

## 当前结论

这一版词表先验证一个最核心的想法：

**只要主词根足够稳定，中文式的词族扩展就会非常快。**

在现有英语里：

- `doctor`
- `hospital`
- `medicine`
- `treatment`
- `medical school`

这些词虽然都属于医学领域，但彼此在字形上没有明显家族感。

而在这套写法里：

- `yi-person`
- `yi-house`
- `yi-skill`
- `yi-study`
- `yi-care`
- `yi-study-house`

它们一眼就能看出是同一语义系统里的词。这正是中文组合方式的优势。

## 下一步建议

下一轮可以继续往四个方向扩：

1. 做 `药` 系词表，例如 `药店 / 药方 / 药效 / 药量`
2. 做 `病` 系词表，例如 `病人 / 病房 / 病史 / 病程`
3. 做 `护` 系词表，例如 `护士 / 护理 / 护工 / 护具`
4. 做 `诊` 系词表，例如 `门诊 / 诊室 / 诊断 / 诊疗`

如果你要，我下一步可以直接继续补第二张表，或者把这一张再扩成 `100` 个医学相关词条。

