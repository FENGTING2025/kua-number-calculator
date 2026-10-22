---
AIGC:
    Label: "1"
    ContentProducer: 001191110102MACQD9K64018705
    ProduceID: 3032888153477379_0-drive/238679272587923369/kua-number-calculator/README.md
    ReservedCode1: ""
    ContentPropagator: 001191110102MACQD9K64028705
    PropagateID: 3032888153477379#1792635268061
    ReservedCode2: ""
---
# Feng Shui Kua Number Calculator 🧭

A free, single-file, zero-dependency Kua (Gua / Ming Gua · 命卦) calculator for the **Eight Mansions (Ba Zhai · 八宅)** school of classical Feng Shui.

**▶ [Open the live calculator](https://fengting2025.github.io/kua-number-calculator/)**

Enter a birth year and gender to instantly see the personal Kua number, trigram, Five Element, East/West group, a color-coded Bagua compass, and the **four auspicious directions** (Sheng Qi, Tian Yi, Yan Nian, Fu Wei) plus the **four cautious directions** (Huo Hai, Wu Gui, Liu Sha, Jue Ming) — each with practical guidance for bed and desk placement. No signup, no tracking, works offline.

## Why this one exists

Most online Kua calculators get the edge cases wrong. This implementation follows the classical formula and the published year tables:

- **Pre-2000:** men subtract the reduced digit from 10; women add 5.
- **2000 and later:** men subtract from 9; women add 6.
- A result of **0 is read as 9** (men born 2000, 2009, 2018, 2027) — a commonly missed rule.
- **Kua 5 has no trigram:** men use Kua 2 (Kun), women use Kua 8 (Gen).
- **Li Chun correction** (~4 February) for January / early-February births.
- Validated against the 1920–2030 year range — every year resolves to a valid Kua (1, 2, 3, 4, 6, 7, 8, 9).

The direction tables follow the Da You Nian Ge (大游年歌) mapping used by the Singapore–Hong Kong tradition, the most common version in English-language references.

## Features

- Pure HTML/CSS/vanilla JavaScript — one `index.html`, no build step, no dependencies
- Color-coded Bagua compass (SVG) with all eight sectors
- Full auspicious/cautious reference tables included on the page
- FAQ with schema.org `FAQPage` structured data for SEO
- Shareable result links (`?y=1990&g=female&l=1`) — prefilled and auto-calculated
- Share buttons for X, Facebook and Reddit; mobile-first responsive design
- No data collection; everything runs in the browser

## Files

- `index.html` — the complete calculator (markup, styles and logic)

## Run locally

Just open `index.html` in any browser, or serve the folder:

```bash
python3 -m http.server 8000
```

## Related free tools

- [Free AI I Ching reading](https://www.askmasterli.com/) — 3 readings per day, traditional three-coin method
- [Chinese Zodiac finder & 2026 fortune](https://www.askmasterli.com/zodiac)
- [All free feng shui & divination tools](https://www.askmasterli.com/tools)
- [`chinese-zodiac-json`](https://github.com/FENGTING2025/chinese-zodiac-json) — structured dataset of the 12 zodiac animals
- [`iching-64-hexagrams-json`](https://github.com/FENGTING2025/iching-64-hexagrams-json) — structured dataset of the 64 hexagrams

## Disclaimer

Traditional cultural guidance for entertainment and personal reflection only. Not a guarantee of outcomes and not professional advice. Regional traditions (Singapore–Hong Kong vs. mainland schools) may differ slightly in formula conventions.

## License

MIT — free for personal and commercial use.

---

> 本内容由 Coze AI 生成，请遵循相关法律法规及《人工智能生成合成内容标识办法》使用与传播。
