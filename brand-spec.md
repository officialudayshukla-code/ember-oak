# Brand spec — Ember & Oak

Placeholder fine-dining brand for a cinematic single-page restaurant site. Visual direction
inverts the Storytelling design system's warm-paper base into its dark counterpart: the
terracotta accent, serif display voice and warm tonal family stay, the ground goes to near-black.

## Tokens (six OKLch bindings, applied in the artifact `:root`)

| Token | Value | Role |
|---|---|---|
| `--bg` | `#0c0a09` | page ground, near-black warm charcoal |
| `--surface` | `#16110e` | cards, panels, form fields |
| `--fg` | `#f6efe6` | primary text, warm off-white |
| `--muted` | `#a2938a` | secondary text, captions, meta |
| `--border` | `#2b2320` | hairlines, dividers, card edges |
| `--accent` | `#c8763f` | single accent — eyebrow, primary CTA, focus ring |

Derived on the spot with `color-mix()`: `--accent-soft`, `--fg-soft`, scrim gradients.

## Type

- Display: `Georgia, 'Times New Roman', serif` — headlines, dish names, prices.
- Body: `Inter, system-ui, sans-serif` — copy, navigation, form labels.
- Mono: `'SF Mono', ui-monospace, Menlo, monospace` — eyebrows, hours, section numerals.

## Observed rules (3–5)

1. One accent only, never more than twice in a viewport: eyebrow label + the single primary CTA.
2. Photographic ground: every section sits on near-black; imagery is the only light source, so
   text over photography is always on a scrim, never on raw pixels.
3. Motion is slow and eased (`cubic-bezier(0.16, 1, 0.3, 1)`, 600–1200ms): parallax drifts,
   reveals rise and unblur, nothing bounces.
4. Rules are hairlines in `--border`; cards have no drop shadows on dark, only a lifted surface.
5. Numerals and small caps are always mono; prices use tabular figures so columns align.