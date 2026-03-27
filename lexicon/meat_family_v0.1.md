# LoongEnglish 第二份词表：肉系 v0.1

这是 `LoongEnglish` 的第二份基础词表，围绕“肉”展开。

这张表的意义非常直接，因为英语在“肉类命名”这件事上，正好存在一块很典型的历史屎山：

- 动物叫 `pig`，但猪肉叫 `pork`
- 动物叫 `cow`，但牛肉叫 `beef`
- 动物叫 `sheep`，但羊肉叫 `mutton`

这对中文使用者并不友好，因为中文的逻辑非常透明：

- 猪 + 肉 = 猪肉
- 牛 + 肉 = 牛肉
- 羊 + 肉 = 羊肉

所以在 `LoongEnglish` 里，这一组词不再沿用历史切裂的英语，而统一改造成：

- `pig-meat`
- `cow-meat`
- `sheep-meat`

也就是：

**词根来自现有英语，组合顺序保留中文。**

## 造词原则

### 1. 主词根来自现有英语

- `meat` = 肉

这里直接选 `meat` 作为“肉”的统一词根。原因很简单：

- 它是现成英语单词
- 语义稳定，识别度高
- 适合和动物词根做高透明组合

### 2. 保持中文组合顺序

统一采用：

- `X + 肉` -> `X-meat`
- `X + 肉 + Y` -> `X-meat-Y`

比如：

- `猪肉` -> `pig-meat`
- `牛肉面` -> `cow-meat-noodle`
- `鸡肉汤` -> `chicken-meat-soup`

### 3. 优先反对历史断裂命名

这张词表的核心态度是：

如果一种英语命名方式无法从表层直接看出和原动物的关系，那它就应该被更透明的中文式组合替代。

所以：

- `pork` 被 `pig-meat` 替代
- `beef` 被 `cow-meat` 替代
- `mutton` 被 `sheep-meat` 替代

## 肉系词表

| 中文词 | 原英语 | LoongEnglish 新词 | 组合拆解 | 说明 |
| --- | --- | --- | --- | --- |
| 肉 | meat | `meat` | 肉 | 食用肉类总词根 |
| 猪肉 | pork | `pig-meat` | 猪 + 肉 | 用动物名直接接 `meat` |
| 牛肉 | beef | `cow-meat` | 牛 + 肉 | 去掉历史断裂词 `beef` |
| 羊肉 | mutton | `sheep-meat` | 羊 + 肉 | 默认按常见羊肉处理 |
| 鸡肉 | chicken | `chicken-meat` | 鸡 + 肉 | 现有英语常省略 `meat`，这里统一补全 |
| 鸭肉 | duck | `duck-meat` | 鸭 + 肉 | 同上，统一显式化 |
| 鱼肉 | fish meat / fish flesh | `fish-meat` | 鱼 + 肉 | 与整鱼 `fish` 区分时更清楚 |
| 鹅肉 | goose meat | `goose-meat` | 鹅 + 肉 | 禽肉类同样统一 |
| 兔肉 | rabbit meat | `rabbit-meat` | 兔 + 肉 | 保持透明组合 |
| 鹿肉 | venison | `deer-meat` | 鹿 + 肉 | 用透明组合替代 `venison` |
| 驴肉 | donkey meat | `donkey-meat` | 驴 + 肉 | 直接组合 |
| 马肉 | horse meat | `horse-meat` | 马 + 肉 | 直接组合 |
| 狗肉 | dog meat | `dog-meat` | 狗 + 肉 | 直接组合 |
| 生肉 | raw meat | `raw-meat` | 生 + 肉 | 状态词前置，保留中文顺序 |
| 熟肉 | cooked meat | `cooked-meat` | 熟 + 肉 | 同上 |
| 鲜肉 | fresh meat | `fresh-meat` | 鲜 + 肉 | 常见描述词组合 |
| 碎肉 | minced meat / ground meat | `cut-meat` | 碎 + 肉 | 强调被切碎后的状态 |
| 肉片 | sliced meat | `meat-slice` | 肉 + 片 | 物体后接形态单位 |
| 肉丝 | shredded meat | `meat-strip` | 肉 + 丝 | 形态细条化 |
| 肉块 | chunk of meat | `meat-block` | 肉 + 块 | 大块肉类表达 |
| 肉末 | minced meat | `meat-dust` | 肉 + 末 | 极细碎状态，偏中式表达 |
| 肉丸 | meatball | `meat-ball` | 肉 + 丸 | 现有英语本就接近中文组合 |
| 肉汤 | meat soup / broth | `meat-soup` | 肉 + 汤 | 食物名组合示例 |
| 肉馅 | meat filling | `meat-fill` | 肉 + 馅 | 包子饺子等馅料表达 |
| 肉酱 | meat sauce | `meat-sauce` | 肉 + 酱 | 调味或浇头类 |
| 牛肉面 | beef noodles | `cow-meat-noodle` | 牛 + 肉 + 面 | 三段组合示例 |
| 猪肉包 | pork bun | `pig-meat-bun` | 猪 + 肉 + 包 | 三段组合示例 |
| 羊肉串 | lamb skewer / mutton skewer | `sheep-meat-stick` | 羊 + 肉 + 串 | 夜市类高频表达 |
| 鸡肉饭 | chicken rice | `chicken-meat-rice` | 鸡 + 肉 + 饭 | 保持结构完整 |
| 肉铺 | butcher shop / meat shop | `meat-shop` | 肉 + 铺 | 场所类组合 |

## 为什么这张表很重要

“肉系”是最适合验证 `LoongEnglish` 价值的一组词，因为它同时满足三点：

- 中文组合极其清晰
- 现有英语历史包袱很重
- 替代后的新词第一眼就能看懂

例如：

- `pork` 不如 `pig-meat` 直观
- `beef` 不如 `cow-meat` 直观
- `venison` 不如 `deer-meat` 直观

这类改造不是搞怪，而是在消除英语里不必要的记忆负担。

## 当前结论

这一版词表说明了一件事：

**只要中文组合关系足够稳定，英语里很多历史遗留词都可以被更透明的结构替换。**

在 `LoongEnglish` 里：

- 动物名负责指明来源
- `meat` 负责指明“食用肉”
- 额外后缀再负责指明形态、做法或菜品

这样整个系统会比现有英语更统一。

## 下一步建议

下一轮可以继续做同一食品方向的词表：

1. `蛋` 系，例如 `鸡蛋 / 鸭蛋 / 蛋黄 / 蛋白`
2. `奶` 系，例如 `牛奶 / 羊奶 / 奶粉 / 奶茶`
3. `面` 系，例如 `面条 / 牛肉面 / 拌面 / 汤面`
4. `饭` 系，例如 `米饭 / 炒饭 / 盖饭 / 盒饭`

如果你要，我下一步可以把“肉系”继续扩成一整套食品词库，并顺手把 `med` 那张表一起整理成统一格式。

