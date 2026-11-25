# Luxury UI design prompt

A single, self-contained LLM prompt that generates **one HTML file**. The file holds a luxury e-commerce interface whose visual language is inspired by the public Louis Vuitton website.

## What the prompt contains

- **Design system.** Colors and typography taken from the official site, each token tagged by provenance: `[verified]`, `[inferred]`, or `[derived]`.
- **UX foundations.** The user's task and the content, browsing and comparing, hierarchy and composition, the states every screen needs, adaptive layout, and accessibility.
- **Interaction polish and motion.** When to animate, easing and duration tokens, choreography, gestures, performance, and reduced motion.
- **Mobile-native details and modern platform features.** `<dialog>`, `popover`, `@starting-style`, and View Transitions.
- **Rules for collisions.** How to resolve conflicts between guidelines, plus a self-check the model runs before it answers.

## Usage

1. Open [`PROMPT.md`](PROMPT.md).
2. Replace `{{BRIEF}}` with what you want designed.
3. Paste the prompt into your model. It returns a single HTML document.

## Disclaimer

This project is not affiliated with Louis Vuitton or LVMH. The prompt asks for original designs only. It explicitly forbids the brand's logo, monogram, Damier pattern, and proprietary typeface.
