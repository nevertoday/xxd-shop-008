---
name: xxd-shop-008
description: "Create XXD Shop 008 miniature brick-world product posters (微缩积木世界商业海报) as finished PNGs from a product photo or product directory, treating the bundled original brief as the sole aesthetic authority: the product rebuilt as a city-scale landmark from standard plastic bricks while staying instantly recognisable with its packaging text, surrounded by scaffolds, cranes, maintenance platforms and busy brick workers, in a matte ABS, brightly lit, vertical commercial composition whose colours grow from the product. Text-free by default (packaging text only), with optional exact user copy. Supports multiple ratios or exact sizes and several compositions per size. Use when the user invokes xxd-shop-008 or asks for 积木风海报、微缩世界、积木工地、产品积木化、乐高风商品图（不使用乐高商标）."
---

# XXD Shop 008｜微缩积木工地

用本次的商品图，把商品变成一座由积木颗粒拼成的巨型地标，周围是正在施工和维护它的微缩积木世界，交付 PNG。

每次生成前，完整读取 `references/original-prompt/zh-CN.md`。这份中文原始提示词是唯一的创作与审美权威；不总结、不翻译、不混用，也不用本文件、README、样张或其他编号替代它。

每次构建生图请求前，完整读取 `references/shop-runtime.md`，它是唯一的家族运行合同。本 Skill 不另写第二套美术指导或运行规则。

所有成品直接写进 `~/Desktop/xxd/xxd-shop-008/` 下新建的一个任务目录（或 `--out` 指定的根目录），不建子目录，不自动拼总览。

## 本编号覆盖条款

**必须有商品图。** 原稿第一句就是“根据用户提供的产品图”，并要求“使人一眼就能认出这是原产品”。没有商品图时只请用户上传。

**原稿规定竖版。** `auto` 推荐 `3:4`（海报、详情页）或 `9:16`（开屏、竖屏信息流）。用户选横版时，说明原稿是“竖版商业广告构图”，巨型产品的地标感会变弱，按用户决定执行。

**只用通用积木，不用任何积木品牌。** 原稿说的是“标准塑料积木颗粒”。凸点上、零件上、包装上都不出现任何真实积木品牌的标识、字样或其专有人仔造型；工人是通用的积木小人。用户说“乐高风”时，理解为这种拼搭风格，商标照样不出现。

**积木化之后包装信息仍要认得出。** 原稿要求“既保留原包装信息，又明显具有积木拼装质感”。Logo、品牌名和主要包装文字要么由颗粒拼出，要么像印刷贴片贴在积木面上，必须可读；脚手架、吊臂和工人不能挡住这些关键信息。

**本编号不问文字方式。** 原稿没有标题或排版逻辑，“按原稿生成”和“不要文字”在这里结果相同：除包装原有文字外不新增任何文字。所以默认按 `--text none` 执行，不问文字方式也不问语言；用户自己给了文案时按 `--text exact` 处理（`--text plan` 同样按 exact），并问一次语言。画面上的字就是商品包装本身；用户的活动标题做成积木或施工告示牌，放在不挡商品的位置，这一句作为用户额外要求追加。

**追加验收：** 商品是画面里最大、第一眼看到的主体；施工叙事是第二眼；所有主体、工人、机械、道路、树木都是积木颗粒质感（天空和空气除外）；没有积木品牌标识；不显得廉价低幼；比例自然，没有失真。

**写入提示词：** 以下句子原话放进交付块的“本编号约束”；其余覆盖条款由 Agent 执行与验收，不进入提示词。

- 不出现任何真实积木品牌的标识、字样或专有人仔造型；工人是由方块拼成的通用积木小人：方形头部、自然肤色、简单方块手，不用圆柱形头、黄色脸或 C 形手的人仔造型。
- 商品包装上的 Logo、品牌名和主要文字积木化之后仍然可读，脚手架、吊臂和工人不挡住它们。
- 品牌名只出现在商品本身；场景里的建筑、底座、招牌和旗帜不另写品牌名或其他文字（用户指定的告示牌文字除外）。

## 参考文件

- `references/shop-runtime.md`：家族运行合同
- `references/original-prompt/zh-CN.md`：运行时使用的原始提示词
- `references/original-prompt/README.md`：译文索引与权威说明
- `references/runtime-preferences.md`：交付偏好沿用
- `references/sample-workflow.md`：仅用于维护样张
- `scripts/configured_imagegen.py`、`scripts/shop_preferences.py`
