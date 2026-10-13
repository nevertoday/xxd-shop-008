<div align="center">

# 🦁 XXD Shop 008 | Miniature Brick Construction Site

### Your product, enlarged into a brick landmark under construction

<a href="README.md">简体中文</a> · <strong>English</strong>

</div>

> Original brief: [Simplified Chinese original](references/original-prompt/zh-CN.md) · [English reading translation](references/original-prompt/en.md)

<!-- xxd-samples:start -->
## Samples

<p align="center"><a href="assets/examples/s01-size-3x4-1086x1448.png"><img src="assets/examples/preview/s01-size-3x4-1086x1448.webp" width="720" alt="Poster"></a><br><sub>Poster · 3:4 · 1086x1448<br>SHANYU coffee beans · <a href="assets/examples/sources/kraft-pouch.jpg">source photo</a> · no added text</sub></p>

### One product, every placement

Same product, same brief: each ratio is a new composition, not a crop.

<table>
<tr><td align="center" valign="top"><a href="assets/examples/s01-size-3x4-1086x1448.png"><img src="assets/examples/preview/s01-size-3x4-1086x1448.webp" height="200" alt="Poster"></a><br><sub>Poster · 3:4 · 1086x1448<br>SHANYU coffee beans · <a href="assets/examples/sources/kraft-pouch.jpg">source photo</a> · no added text</sub></td><td align="center" valign="top"><a href="assets/examples/s02-size-9x16-941x1672.png"><img src="assets/examples/preview/s02-size-9x16-941x1672.webp" height="200" alt="Splash screen"></a><br><sub>Splash screen · 9:16 · 941x1672<br>SHANYU coffee beans · <a href="assets/examples/sources/kraft-pouch.jpg">source photo</a> · no added text</sub></td><td align="center" valign="top"><a href="assets/examples/s03-size-2x3-1024x1536.png"><img src="assets/examples/preview/s03-size-2x3-1024x1536.webp" height="200" alt="Outdoor vertical banner"></a><br><sub>Outdoor vertical banner · 2:3 · 1024x1536<br>SHANYU coffee beans · <a href="assets/examples/sources/kraft-pouch.jpg">source photo</a> · no added text</sub></td><td align="center" valign="top"><a href="assets/examples/s04-size-4x5-1122x1402.png"><img src="assets/examples/preview/s04-size-4x5-1122x1402.webp" height="200" alt="Social post"></a><br><sub>Social post · 4:5 · 1122x1402<br>SHANYU coffee beans · <a href="assets/examples/sources/kraft-pouch.jpg">source photo</a> · no added text</sub></td></tr>
</table>

### Across categories

<table>
<tr><td align="center" valign="top"><a href="assets/examples/s05-category-9x16-941x1672.png"><img src="assets/examples/preview/s05-category-9x16-941x1672.webp" height="220" alt="Splash screen"></a><br><sub>Splash screen · 9:16 · 941x1672<br>LENGCHUAN sugar-free sparkling water · <a href="assets/examples/sources/black-can.jpg">source photo</a> · no added text</sub></td><td align="center" valign="top"><a href="assets/examples/s06-category-3x4-1086x1448.png"><img src="assets/examples/preview/s06-category-3x4-1086x1448.webp" height="220" alt="Poster"></a><br><sub>Poster · 3:4 · 1086x1448<br>YEFENGPO wildflower honey · <a href="assets/examples/sources/honey-jar.jpg">source photo</a> · no added text</sub></td></tr>
</table>

### Campaign sign

<table>
<tr><td align="center" valign="top"><a href="assets/examples/s07-special-3x4-1086x1448.png"><img src="assets/examples/preview/s07-special-3x4-1086x1448.webp" height="220" alt="Poster"></a><br><sub>Poster · 3:4 · 1086x1448<br>LENGCHUAN sugar-free sparkling water · <a href="assets/examples/sources/black-can.jpg">source photo</a> · exact copy (Chinese)</sub></td></tr>
</table>

<sub>All sample products are fictional demo brands, and their prices and specs are demo values. Source photos come from Unsplash; credits and licence are in [assets/examples/README.md](assets/examples/README.md). Each image is one complete generation: not retouched, composited or upscaled, with its real pixel size shown. Images that failed visual review were regenerated and are not shown. Click for full size.</sub>

<!-- xxd-samples:end -->

## What it solves

Launches, collaborations and seasonal key visuals need an image people stop to explore. A plain product shot cannot do it; pure 3D cartoons make the product unrecognisable.

**Shop 008** tells a tiny story: the product, rebuilt from plastic bricks at city scale, stands at the centre of a miniature world with scaffolds, cranes and maintenance platforms, while brick workers carry, polish, wipe, post and inspect. First glance: the giant product, instantly recognisable. Second glance: what the little workers are doing.

## About "LEGO style"

It is a building style, not a brand. No real brick brand's logo, wordmark or proprietary minifigure design appears anywhere, studs included.

## Getting started

```bash
git clone https://github.com/nevertoday/xxd-shop-008.git
ln -s "$(pwd)/xxd-shop-008" ~/.claude/skills/xxd-shop-008
```

```text
/xxd-shop-008 ./sparkling-water.png --size 3:4 --text none
/xxd-shop-008 ./tumbler.png --size 9:16 --text exact --copy "Under construction · opens Sept 20" --locale en-US
```

Key flags: `--size` (the brief is vertical), `--count`, `--text none / exact`, `--locale`. Full list in the [family runtime](references/shop-runtime.md).

## Boundaries

- A product photo is required; logo, brand name and main packaging text stay legible and unblocked.
- The original brief is kept verbatim and is the only aesthetic authority.

<!-- xxd-shop-tail -->
## Project structure

```text
xxd-shop-008/
├── SKILL.md
├── README.md / README.en.md
├── LICENSE
├── agents/openai.yaml
├── assets/examples/
├── scripts/
│   ├── configured_imagegen.py
│   └── shop_preferences.py
└── references/
    ├── shop-runtime.md
    ├── runtime-preferences.md
    ├── sample-workflow.md
    └── original-prompt/
        ├── README.md
        ├── zh-CN.md
        └── en.md
```

<!-- xxd-readme-ads:start -->
## About XXD

XXD is Xiaoxiaodong's abbreviated brand name. This project is created and maintained by [@xiaoxiaodong01](https://x.com/xiaoxiaodong01).

## Xiaoxiaodong multi-platform membership · CNY 699/year

> **Advertising disclosure:** The QR code, membership, and paid-service links below are XXD promotional information. Scanning or purchasing is entirely optional and does not affect access to this open-source project.

One annual membership unlocks three benefits together: **Knowledge Planet + the XXD Member Prompt Library + membership for all General Skills**. They are included in one membership; no separate purchase is required.

<!-- xxd-shop-command-system:start -->

### How the Skills work together

| Level | Included | What it does |
|---|---|---|
| **General** | `xxd-shop-all` | Detects available numbered Skills, recommends them by product, placement and visual need, and organizes multi-style and batch tasks. |
| **Soldier** | `xxd-shop-NNN` | Each numbered Skill follows its own original brief and aesthetic to complete the specific task assigned by the General. |

<!-- xxd-shop-command-system:end -->

### What you receive

1. **One-to-one WeChat AI learning and project support**
   Add Xiaoxiaodong on WeChat via the QR code below to discuss AI learning, tools, and real projects one to one, with practical guidance and answers. Representative questions may be organized into member resources.
2. **A growing member prompt library**
   The [XXD Member Prompt Library](https://vip.xiaoxiaodong.ai/) currently contains about 32,000 prompts and will keep expanding, with a goal of exceeding 100,000.
3. **All General Skills and usage support**
   One membership covers every General Skill, with usage guidance and Q&A when you need help.
4. **Priority for high-need requests**
   Frequently requested, high-need prompts and Skills are reviewed and developed first where appropriate.

### How to join

- [Activate membership on the member website](https://vip.xiaoxiaodong.ai/).
- Or scan the QR code below to add Xiaoxiaodong on WeChat for one-to-one activation support.

<p align="center"><a href="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png"><img src="https://xiaoxiaodong.pages.dev/assets/wechat-qr.png" alt="Contact Xiaoxiaodong" width="280"></a></p>
<!-- xxd-readme-ads:end -->

## License

This project—including its Skill, prompts, scripts, documentation, and accompanying samples—is released under the **PolyForm Noncommercial License 1.0.0**. The complete legal text is in [LICENSE](LICENSE); the official page is <https://polyformproject.org/licenses/noncommercial/1.0.0>.

In plain language:

- You may use it for personal study, research, experiments, testing, hobbies, and private entertainment. Charities, educational institutions, public research/safety/health organisations, environmental-protection organisations, and government institutions may also use it.
- For **noncommercial purposes**, you may use, copy, modify, create derivative works, and share the project. When sharing, include this license (or the link above) and every `Required Notice:` line supplied by the author.
- Commercial products or services, paid delivery, selling access or licenses, and uses with an anticipated commercial application are not allowed. Obtain separate written permission from the copyright holder for commercial use.
- The license grants only the stated copyright and limited patent rights. It grants no trademark, brand, or other unstated rights, and you may not sublicense or transfer your license.
- If you receive written notice of a violation, you have 32 days to come into full compliance and take practical corrective steps; otherwise the licenses end. A written patent-infringement claim also ends the patent license.
- The project is provided **as is**, without warranties, and you accept the risks and any resulting liability to the extent permitted by law.
