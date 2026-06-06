---
name: presentation
description: 'Use when asked to create or update presentation. Does creates presentation according to the given instructions. USE FOR: new presentations, updating existing presentations, and improving existing presentations.'
---

# Presentation

Self-contained HTML slide decks. One `.html` file per deck, keyboard-navigated, no build step.

## Principles

- Keep it simple. Minimal content per slide — one idea, a few lines.
- No images. Use type, layout, and code blocks for visual interest.
- Consistency over decoration. Every deck shares the same fonts, colors, and components.

## Structure

- One `.html` file per presentation, named `YYYY-topic.html`.
- Each slide is a `<section class="slide">`. First slide has `active`.
- Inline `<style>` and `<script>` — no external CSS/JS except the font.

## Style

- Font: `JetBrains Mono` (Google Fonts), monospace everywhere.
- Theme: dark. `--bg: #0a0a0a`, `--fg: #fafafa`, `--border: #2a2a2a`.
- Links: `inherit` color, underlined.
- Type scale via utility classes: `t-xl`, `t-lg`, `t-md`, `t-year`, `t-lede`, `t-body`, `t-note`, `t-label`, `t-cap`.
- Layout via `stage` flex container + modifiers: `center`, `bottom`, `col`, `between`, `end`, `middle`, `gap-*`.
- Code via `pre.code` (+ `sm`, `lg`, `tight`, `wrap`). Wrap highlighted tokens in `<span>`.

## Workflow

1. Copy an existing deck (e.g. `2026-agent-skills.html`) as the starting point.
2. Reuse its `<style>` block verbatim — do not introduce new fonts or colors.
3. Write slides as `<section class="slide">`, one idea each.
4. Keep the navigation `<script>` unchanged.
5. Open in a browser and step through with arrow keys to verify.