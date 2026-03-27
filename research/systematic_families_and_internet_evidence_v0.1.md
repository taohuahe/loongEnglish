# LoongEnglish 研究笔记：中文成体系、英语不成体系的词族梳理 + 互联网证据

## 结论先行

如果从 `LoongEnglish` 的角度看，最值得优先改造的，不是零散单词，而是**中文里已经有稳定组合逻辑、但英语里要么历史断裂、要么命名分散、要么只能靠长短语拼补**的整组词族。

这类词族大致有四种英语问题：

1. **历史断裂**
   例如 `猪肉 / 牛肉 / 羊肉` 对应 `pork / beef / mutton`
2. **同根消失**
   例如 `学 / 学生 / 学校 / 学费 / 学术` 在英语里变成 `study / student / school / tuition / academic`
3. **词义压扁**
   例如中文亲属词很细，英语大量压成 `uncle / aunt / cousin`
4. **只能靠短语补洞**
   例如 `前天 / 后天 / 大后天`，英语缺少同级单词系统

对项目来说，最有价值的是第一类和第二类，因为最适合做“英语词根 + 中文组合”的系统改造。

## 一、候选词族总表

下面这张表优先从“适合做词库”和“容易被人第一眼看懂”两个维度排序。

| 优先级 | 中文词族 | 中文里的系统性 | 英语里的断裂方式 | 适合度 | 已找到类似用法证据 |
| --- | --- | --- | --- | --- | --- |
| A | 医 | 医、医生、医院、医学、医疗、医保、医护 | `doctor / hospital / medicine / treatment / insurance` 分散 | 很高 | 强 |
| A | 肉 | 猪肉、牛肉、羊肉、鹿肉、兔肉 | `pork / beef / mutton / venison` 历史断裂 | 很高 | 强 |
| A | 奶 | 牛奶、羊奶、驴奶、奶粉、奶酪 | `milk / dairy / formula / cheese` 不同层级混用 | 很高 | 强 |
| A | 学 | 学生、学校、学费、学术、学位、学科 | `student / school / tuition / academic / degree / discipline` 分散 | 很高 | 中 |
| A | 费 | 水费、电费、车费、会费、路费、学费 | `fee / fare / dues / toll / bill / tuition` 混杂 | 很高 | 强 |
| A | 证 / 卡 | 学生证、工作证、借书证、医保卡、门卡 | `ID / card / badge / certificate / license` 混杂 | 很高 | 强 |
| A | 网 | 网民、网友、网课、网店、网红、网银 | `netizen / online course / online store / internet celebrity / online banking` 半系统 | 很高 | 强 |
| A | 房 / 室 | 卧室、教室、病房、诊室、浴室、书房 | `bedroom / classroom / ward / clinic room / bathroom / study` 半系统 | 很高 | 中 |
| A | 车 | 火车、校车、货车、客车、救护车、自行车 | `train / school bus / truck / coach / ambulance / bicycle` 分散 | 很高 | 中 |
| A | 病 | 病人、病房、病历、病史、病因、病情 | `patient / ward / record / history / cause / condition` 分散 | 很高 | 中 |
| B | 法 | 法律、法院、法官、法学、法条、法务 | `law / court / judge / jurisprudence / statute / legal` 分散 | 高 | 弱 |
| B | 院 | 医院、法院、学院、戏院、研究院 | `hospital / court / college / theatre / institute` 分散 | 高 | 弱 |
| B | 机 | 手机、相机、打印机、洗衣机、耳机、主机 | `phone / camera / printer / washer / headphones / host` 分散 | 高 | 弱 |
| B | 台 | 前台、后台、阳台、讲台、舞台、窗台 | `front desk / backstage / balcony / podium / stage / sill` 分散 | 高 | 中 |
| B | 口 | 入口、出口、门口、路口、港口 | `entrance / exit / doorway / intersection / port` 分散 | 高 | 中 |
| B | 站 | 车站、网站、地铁站、基站、站点 | `station / site / stop / base station / node` 分散 | 高 | 中 |
| B | 线 | 电线、网线、电话线、火线、底线、支线 | `wire / cable / line / frontline / bottom line / branch line` 混杂 | 高 | 中 |
| B | 单 | 菜单、账单、清单、表单、名单、运单 | `menu / bill / checklist / form / roster / waybill` 分散 | 高 | 中 |
| B | 护 | 护士、护理、护栏、护具、防护 | `nurse / nursing / guardrail / protective gear / protection` 分散 | 高 | 弱 |
| B | 用 | 医用、军用、家用、商用、民用 | `medical-use / military / household / commercial / civilian` 部分共形、部分断裂 | 高 | 中 |
| C | 亲属 | 伯父、叔父、舅舅、姨妈、表哥、堂姐 | 英语大量压成 `uncle / aunt / cousin` | 中高 | 中 |
| C | 相对时间 | 前天、昨天、今天、明天、后天、大后天 | 英语只能部分单词化，后面靠短语补 | 很高 | 弱 |
| C | 星期 / 月份 | 星期一到星期日，一月到十二月 | 英语名称历史性强，不透明 | 高 | 弱 |
| C | 公 | 公交、公厕、公园、公费、公路、公安 | `bus / public toilet / park / public expense / highway / police` 混杂 | 中 | 弱 |
| C | 文 / 语 | 中文、英文、法文、原文、译文、语法 | `Chinese / English / French / original text / translation / grammar` 分散 | 中 | 弱 |

## 二、最值得先做的 12 组

如果你要继续做词库，建议先按下面的顺序推进。

### 1. 肉系

这是最典型的英语历史断裂区。

- 中文：`猪肉 / 牛肉 / 羊肉 / 鹿肉`
- 英语：`pork / beef / mutton / venison`
- LoongEnglish 潜力：`pig-meat / cow-meat / sheep-meat / deer-meat`

优势：

- 一眼就懂
- 改造收益极高
- 互联网已经有大量现成透明用法

### 2. 医系

这个词族的痛点不是缺词，而是**没有显式同根**。

- 中文：`医生 / 医院 / 医学 / 医疗 / 医保`
- 英语：`doctor / hospital / medicine / treatment / insurance`
- LoongEnglish 潜力：`med-person / med-house / med-study / med-care / med-cover`

优势：

- 适合 AI 学习
- 适合做行业词族
- 已经有 `med school / med student / Penn Medicine` 这类真实世界前例

### 3. 费系

中文的 `X费` 非常统一，但英语被拆成一堆不同词。

- 中文：`水费 / 电费 / 学费 / 会费 / 路费 / 车费 / 停车费`
- 英语：`water fee / electricity bill / tuition / membership fee / toll / fare / parking fee`

LoongEnglish 可以尝试统一为：

- `water-fee`
- `power-fee`
- `study-fee`
- `member-fee`
- `road-fee`
- `car-fee`

### 4. 证 / 卡系

中文对“证件”处理得很稳定，英语则在 `card / ID / badge / certificate / license` 之间跳。

- 中文：`学生证 / 工作证 / 借书证 / 结婚证 / 驾驶证 / 医保卡`
- 英语：`student card / employee ID / library card / marriage certificate / driver's license / health card`

LoongEnglish 可以统一考虑：

- `student-card`
- `work-card`
- `library-card`
- `marry-card`
- `drive-card`
- `health-card`

### 5. 网系

这个词族很适合扩散，因为互联网英语本来就处于快速演化状态。

- 中文：`网民 / 网友 / 网课 / 网店 / 网红 / 网银 / 网盘`
- 英语：`netizen / online friend / online course / online store / internet celebrity / online banking / cloud drive`

LoongEnglish 潜力：

- `net-friend`
- `net-course`
- `net-store`
- `net-bank`
- `net-red` 或更英语化的 `net-star`

### 6. 奶系

奶类在全球英语里已经大量使用动物名 + `milk`，这说明透明组合天然有可接受性。

- 中文：`牛奶 / 羊奶 / 驴奶 / 奶粉 / 奶酪`
- 英语：`cow milk / goat milk / donkey milk / formula / cheese`

LoongEnglish 可以继续把这一组统一下去。

### 7. 房 / 室系

英语里其实已经有 `bedroom / classroom / bathroom / study room`，但它不完整。

- 中文：`卧室 / 教室 / 诊室 / 病房 / 书房 / 厨房`
- 英语：`bedroom / classroom / exam room / ward / study / kitchen`

适合把断掉的地方补回去。

### 8. 车系

英语对交通工具命名是多种历史路线混在一起的结果。

- 中文：`火车 / 校车 / 货车 / 客车 / 救护车 / 自行车`
- 英语：`train / school bus / truck / coach / ambulance / bicycle`

LoongEnglish 潜力很大，但要先选好统一后缀，是 `car`、`truck`、`bus` 还是更抽象的 `ride / vehicle`。

### 9. 学系

这是一个非常大的概念簇。

- 中文：`学 / 学生 / 学校 / 学费 / 学术 / 学位 / 学科`
- 英语：`study / student / school / tuition / academic / degree / discipline`

问题不在于英语没有这些词，而在于它们**不是一个形态家族**。

### 10. 病系

- 中文：`病人 / 病房 / 病历 / 病史 / 病因 / 病情`
- 英语：`patient / ward / medical record / medical history / cause / condition`

适合和医系联动。

### 11. 台系

- 中文：`前台 / 后台 / 讲台 / 舞台 / 阳台 / 窗台`
- 英语：`front desk / backend / podium / stage / balcony / windowsill`

这里英语不是没表达，而是缺少共享词根。

### 12. 相对时间系

- 中文：`前天 / 昨天 / 今天 / 明天 / 后天 / 大后天`
- 英语：`the day before yesterday / yesterday / today / tomorrow / the day after tomorrow`

这是中文对英语的一个明显降维打击区。问题是这组虽然很有价值，但现成英语证据弱，改造难度比肉系、医系更大。

## 三、互联网已找到的类似用法证据

这里的“类似用法”分四种，不要混在一起看：

1. **标准英语现成表达**
2. **机构或行业缩略表达**
3. **全球英语 / 非美式英语中的透明组合**
4. **受翻译或跨语言影响而固定下来的表达**

### A. 医系：已有强证据

证据类型：机构缩略 + 标准化品牌用法

- `med` 本身已被 `Merriam-Webster` 收为 `medical` 的缩略形式  
  https://www.merriam-webster.com/dictionary/med
- Stanford 官方新闻标题直接使用 `med school`  
  https://med.stanford.edu/news/all-news/2018/09/new-med-school-curriculum-expands-opportunities-for-research.html
- `Penn Medicine` 是正式机构品牌  
  https://www.pennmedicine.org/

判断：

- `med` 在英语世界不是陌生音节
- 它确实能做词根
- 但它更像“被认可的短词根”，不是可无限自由组合的普通词

### B. 肉系：已有强证据

证据类型：行业英语 + 国际农业 / 食品体系用语

- FAO 使用 `pig meat`  
  https://www.fao.org/4/y4252e/y4252e05b.htm
- FAO 页面出现 `cow meat`  
  https://www.fao.org/4/Y4732E/y4732e09.htm
- FAO 与相关机构大量使用 `sheep meat`  
  https://www.fao.org/family-farming/detail/en/c/1398993/
- USDA FSIS 官方页面使用 `goat meat`  
  https://www.fsis.usda.gov/food-safety/safe-food-handling-and-preparation/meat-catfish/goat-farm-table
- 美国肉类出口手册里有 `Boneless Sheep Meat`  
  https://usmef-prod-clients-avibeweb.s3.amazonaws.com/files/BDFF5A9D-94C9-4FD1-A70F-C3A0BB2F6AAB.pdf

判断：

- `pig meat / sheep meat / goat meat / deer meat / cow meat` 并不是幻想词
- 它们已经在国际农业、贸易、检验和食品环境里真实存在
- 但在美国日常消费英语里，`beef / pork / lamb` 仍然更主流

### C. 奶系：已有强证据

证据类型：农业和乳业标准表达

- FAO `Milk composition` 页面直接使用 `cow milk`、`sheep milk`  
  https://www.fao.org/dairy-production-products/products/milk-composition/
- FAO `Small ruminants` 页面大量使用 `goat milk`、`sheep milk`  
  https://www.fao.org/dairy-production-products/dairy/small-ruminants/en
- FAO 新闻中有 `goat milk`  
  https://www.fao.org/africa/news-stories/news-detail/mauritius-promotes-goat-milk-to-strengthen-food-security-and-rural-livelihoods/en

判断：

- `X-milk` 在英语世界接受度很高
- 说明“动物名 + 产品名”的透明组合是可行的
- 奶系适合优先纳入词库

### D. 证 / 卡系：已有强证据

证据类型：机构日常英语

- University of Edinburgh 官方使用 `student card`  
  https://www.ed.ac.uk/students/new-students/online-students/getting-started/apply-for-and-receive-your-university-student-card
- Canada 官方使用 `health card`  
  https://www.canada.ca/en/health-canada/services/health-care-system/canada-health-care-system-medicare/provincial-territorial-health-care-resources.html
- Dallas Public Library 官方使用 `library card`  
  https://www.dallaslibrary.org/services/library-card
- University of North Alabama 官方 PDF 使用 `employee ID card`，并同时提到 `student card` / `library card`  
  https://www.una.edu/employee-policy-manual/3general_info_and_statements/identification_cards.pdf

判断：

- `X-card` 在英语里已经很自然
- 问题不是能不能用，而是英语没有把所有证件都统一挂在一个后缀上
- 这个词族很适合做系统化收编

### E. 费系：已有强证据

证据类型：政府 / 城市收费文件

- Portland 官方页面使用 `parking fee`  
  https://www.portland.gov/transportation/40219
- Saint Paul Regional Water Services 使用 `water service base fee`  
  https://www.stpaul.gov/departments/saint-paul-regional-water-services/billing-and-payment/rates-and-fees
- Canada 官方页面使用 `membership fees`  
  https://www.canada.ca/en/revenue-agency/services/charities-giving/charities/policies-guidance/summary-policy-m05-membership-fees.html
- University of Oklahoma 页面使用 `Registration Fee`，并提到在线课程收费  
  https://www.ou.edu/pacs/edi/online-courses.html

判断：

- `X-fee` 在英语里大量存在
- 但英语同时还有 `dues / fare / tuition / toll / bill / rate`
- 这说明“费系”不是不能造，而是存在大量旧体系竞争

### F. 网系：已有强证据

证据类型：词典收录 + 大学 / 银行正式用法

- `netizen` 被 `Merriam-Webster` 收录  
  https://www.merriam-webster.com/dictionary/netizen
- Marshall University 官方定义 `online course`  
  https://www.marshall.edu/online/disclaimers-and-definitions/
- Chase 官方使用 `Online Banking`  
  https://www.chase.com/digital/online-banking
- Bank of America 官方使用 `Mobile and Online Banking`  
  https://info.bankofamerica.com/en/digital-banking

判断：

- `net- / online / internet-` 已经是英语里真实存在的网络语义前缀
- 问题在于它们没有被统一成一个稳定词根体系
- 网系是最适合用 AI 扩散的领域之一

### G. 车系：已有中强证据

证据类型：标准英语复合词

- NHTSA 官方大量使用 `school bus`  
  https://www.nhtsa.gov/school-bus-regulations-faqs
- `fire truck` 被 `Merriam-Webster` 收录  
  https://www.merriam-webster.com/dictionary/fire%20truck

判断：

- 英语并不是完全不能做 `X + vehicle` 组合
- 只是这套组合没有覆盖整个交通工具系统
- 因此车系有潜力，但设计上要更慎重

### H. 亲属系：有部分证据，但自然度不稳定

证据类型：描述性短语存在，但缺少标准单词体系

- `elder brother` 被 `Merriam-Webster` 和 Cambridge 例示承认  
  https://www.merriam-webster.com/dictionary/elder  
  https://dictionary.cambridge.org/us/dictionary/essential-american-english/elder
- Washington 州卫生部门术语表使用 `paternal uncle`  
  https://doh.wa.gov/sites/default/files/2024-03/344085-GeneticsGlossary.pdf
- Cambridge 对 `uncle` 的定义仍然是父母任一方的兄弟，粒度明显更粗  
  https://dictionary.cambridge.org/us/dictionary/essential-british-english/uncle

判断：

- 英语能描述，但经常只能靠补充修饰语
- 亲属系很适合做中文优势展示
- 但如果想做成自然英语，需要更长时间打磨

## 四、我对“是否已经有人这么说”的判断

可以把现在互联网上的证据分成三个等级。

### 强

说明：已经是自然英语或稳定机构英语。

- `med`
- `med school`
- `Penn Medicine`
- `student card`
- `health card`
- `library card`
- `parking fee`
- `membership fee`
- `netizen`
- `online course`
- `online banking`
- `school bus`
- `fire truck`
- `goat milk`
- `cow milk`
- `sheep milk`

### 中

说明：真实存在，但更偏行业、地区或国际英语，不一定是美国普通人最常用的默认说法。

- `pig meat`
- `cow meat`
- `sheep meat`
- `deer meat`
- `water fee`
- `work card`
- `internet celebrity`
- `study room`
- `exam room`

### 弱

说明：中文逻辑很强，但我这轮没有找到足够强的自然英语证据，或者英语更多靠解释性短语。

- `前天 / 后天 / 大后天`
- `星期一 / 星期二` 这类编号星期
- `一月 / 二月` 这类编号月份
- `伯父 / 叔父 / 舅舅 / 姨夫 / 堂哥 / 表哥` 这类高精度亲属词

## 五、对项目的具体建议

### 1. 先做“高透明 + 高证据”词族

建议优先顺序：

1. 肉
2. 奶
3. 医
4. 费
5. 证 / 卡
6. 网

这几组最容易让人一眼懂，而且互联网上已经能找到现成前例。

### 2. 把“已有真实英语前例”的词单独标出来

建议后续每个词条增加一列：

- `evidence_level = strong / medium / weak`

这样后面做扩散时可以区分：

- 是“已有英语前例，LoongEnglish 负责系统化”
- 还是“完全新造，LoongEnglish 负责首次提出”

### 3. 不要把所有词族一把梭统一

有些词族适合统一，例如：

- 肉
- 奶
- 费
- 卡

有些词族则要谨慎，例如：

- 车
- 亲属
- 时间

因为它们涉及更强的文化约定和历史惯性。

### 4. 下一份研究最值得做什么

如果继续推进，我建议下一轮直接输出三份东西：

1. `top_100_systematic_families.md`
   把最有价值的 100 个中文系统词族列全
2. `evidence_matrix.csv`
   每个词族对应“是否已见互联网真实用法”
3. `lexicon_food_v0.1.md`
   先把 `肉 / 奶 / 蛋 / 面 / 饭` 做成一个完整的食品词库

## 六、当前最强的一句项目规则

这轮研究之后，项目规则可以进一步明确成一句话：

**LoongEnglish 优先改造那些“中文内部已经高度系统化、但英语仍然碎片化”的词族，并优先吸收互联网上已经出现的透明组合用法。**

