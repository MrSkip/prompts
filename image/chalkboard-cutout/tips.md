# Tips — Chalkboard Cutout

## Aspect ratio

- `--ar 1:1` — square (default, good for social).
- `--ar 2:3` — vertical poster, gives room for tall decorations.
- `--ar 3:2` — landscape, good when the chalk body extends sideways.

## Midjourney

- Add `--style raw` so MJ doesn't over-stylize the photoreal head.
- Append `--no color, painted, 3d render` if chalk drawings come out
  tinted or look CGI-rendered.
- For tighter control over chalk style, add `--sref <url>` pointing to
  a real chalkboard-art reference image.

## DALL-E 3 / GPT image

- Append "in the style of chalkboard art mixed with portrait photography"
  if the model struggles to combine the two materials.
- DALL-E under-delivers on photoreal heads by default. Be explicit:
  *"magazine-quality portrait, 85mm lens, retouched skin detail."*

## Common failure modes

- **Sketchy head**: model draws the head in chalk too. Fix: emphasize
  *"magazine portrait quality"* or *"85mm lens, sharp focus"* for the head.
- **Painted/colored chalk body**: model treats chalk outlines as a color
  to fill. Fix: *"pure white chalk lines only, no fill, shading only in
  white chalk hatching."*
- **Paste-up look**: head sits on the body unnaturally. Fix: insist on
  unified spotlight lighting tinting both layers.
- **Cluttered frame**: every corner is full of decorations. Fix: name
  specific decorations (max 5) and add *"leave negative space."*
- **Wrong typography style**: text comes out printed/sans-serif. Fix:
  *"hand-lettered chalk script with imperfect strokes, slight smudging."*
