# Luxury HTML deck prompt

A single, self-contained LLM prompt that generates a **slide deck as one HTML file**. The deck works as a live presentation in the browser, and it is built to be **converted to PPTX** later with tools such as html2pptx, pptxgenjs, or python-pptx. Its visual language is inspired by the public Louis Vuitton website.

## What the prompt contains

- **Design system:** the real colors of the official site, each tagged by provenance (`[verified]`, `[inferred]`, `[derived]`), plus a type scale for projection with a single 400 weight.
- **Conversion contract:** fixed 1280×720 slides, text kept in semantic elements only, no gradients, transforms, or pseudo-element text, charts as inline SVG, and speaker notes in `aside.notes`.
- **12 slide layouts:** title, agenda, section divider, content, two columns, KPI, quote, visual, chart, table, process, and closing.
- **Storytelling rules:** one idea per slide, action titles, bullet limits, and charts with direct labels.
- **Presentation mode:** a progressive layer that never changes the static DOM. It covers keyboard and click navigation, `#slide-N` deep links, fullscreen, the notes panel, the export view, and printing to PDF.
- **Quality rules:** restrained motion, accessibility, rules for resolving conflicts, and a self-check.

## Usage

1. Paste [`PROMPT.md`](PROMPT.md) into your model as the first message. It replies `Ready. Send the presentation instruction.`
2. Send the presentation you want as the next message. The model returns a single HTML file.
3. Open the file to present it, add `?export` to the URL to see every slide stacked for conversion, or print it to PDF.

## Disclaimer

This project is not affiliated with Louis Vuitton or LVMH. The prompt asks only for original designs. It forbids the brand's logo, monogram, Damier pattern, and proprietary typeface.
