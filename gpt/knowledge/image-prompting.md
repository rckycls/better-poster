# Image prompting

How to write prompts for the image tool that produce specific, designed-looking posters, with accurate text.

## Prompt anatomy

Write the prompt in this order, in plain sentences. Be specific and physical: describe the object you'd hold in your hand, not adjectives about how good it is.

1. **Artifact and process:** what the thing physically is. "A two-color screen-printed poster on cream uncoated paper." "A hand-painted sign on a white board." "A photo of a printed menu card lying on a marble counter" (only if a photographed mockup is wanted).
2. **Format:** orientation and aspect. "Portrait poster, 2:3."
3. **Layout:** where things go, in grid terms. "Headline set huge across the top third, flush left. Illustration of the bun in the lower right, cropped by the edge. Small info block bottom left."
4. **Text:** every word that should appear, in double quotes, in reading order, with its role and look.
   - `Headline: "CARDAMOM BUNS" in tall condensed bold sans, black.`
   - `Below it, smaller: "Saturdays from 8am".`
   - `Bottom left, small: "Holm Bakery · 41 Dock St".`
   - End with: `No other text anywhere.`
5. **Imagery:** the specific subject. Name the product, how it looks, and what it sits on. "A single cardamom bun, twisted knot shape, pearl sugar on top, on a sheet of baking paper."
6. **Palette:** 2–4 named colors, with hex values if you have them. "Only three colors: cream paper, black, and tomato red."
7. **Texture and finish:** grain, ink bite, misregistration, brush strokes, film grain, toner noise.
8. **Exclusions:** what not to include. "No gradients, no drop shadows, no sparkles, no extra decorations, no other text."

## Text-rendering rules

The image tool can render text well but makes mistakes as text gets longer and smaller.

- Keep the image route to about 20 words or fewer, in at most 4 text blocks. More than that → layout route (menu-design.md).
- Put every string in double quotes exactly as it should appear, with the correct capitalization.
- Write prices and times exactly as they should look: "$4.50", "8am–2pm", "Sat 14 June".
- Spell unusual words carefully. If a word keeps coming out wrong, simplify it or move it to a separate layout.
- Always add "No other text anywhere." to prevent gibberish fillers.
- Give text its own clear area of flat color. Text over a busy image fails more often and reads worse.
- After generating, read every word in the image. Fix any errors with an edit ("change the price to "$4.50", keep everything else exactly the same") before showing it.

## Sizes

| Use | Aspect | Notes |
|---|---|---|
| Poster, flyer, window sign | Portrait 2:3 | A-series and US Letter are close to this; leave margin so trimming is safe |
| Instagram feed | Portrait 2:3 or square | Feed crops to 4:5; keep key content away from top and bottom edges |
| Instagram / WhatsApp story | Portrait 2:3 | Story is 9:16; keep text in the middle, add top and bottom background when posting |
| TV menu board, banner, website header | Landscape 3:2 | Keep text large; viewed from far away |

Generated images are about 1024×1536 px. That's fine for screens and for prints up to about A5 / half-letter. Be honest about this. For A4/Letter or larger prints, use the layout route (sharp text at any size) with the generated artwork as a background, or recommend upscaling the image.

## Using the user's images

- **Storefront, interior or products:** pull palette, materials and real details from them ("the green tile from your counter", "your blue cups").
- **Product photo as reference:** "Illustrate this exact pastry from the attached photo as a linocut" works better than describing it.
- **Logos:** the image tool redraws logos and usually distorts them. Leave a clean space for the logo ("keep the top-left corner empty, flat cream, for a logo") and tell the user to place it, or use the layout route, which inserts the real file.

## Editing and iterating

- Change one or two things at a time and say "keep everything else exactly the same".
- Reuse your last prompt and edit it; don't rewrite from scratch, or the design will drift.
- For a set (poster + story + menu), keep the artifact, palette, type description and texture wording identical across prompts.

## Example prompts

### Bakery weekend special (linocut)

> A hand-carved linocut print, portrait 2:3, printed in two inks, black and tomato red #D9442B, on cream uncoated paper #EFE6D2. Upper two-thirds: a large linocut illustration of a single cardamom bun, twisted knot shape with pearl sugar on top, sitting on a crumpled sheet of baking paper, bold gouge marks, carved in black with the paper's cream showing through. Bottom third, flush left, carved block lettering: headline "CARDAMOM BUNS" in red, large. Under it in black, smaller: "Saturdays from 8am". Bottom right, small black text: "Holm Bakery, 41 Dock St". No other text anywhere. Uneven inking with small white specks, slight ink bite into the paper. No gradients, no shadows, no decorative borders.

### Taqueria Tuesday deal (hand-painted sign)

> A hand-painted sign on a flat white wooden board, portrait 2:3, by a traditional sign painter. Top: "TACO TUESDAY" in red brush-lettered block capitals with a painted black drop shade, filling the width. Middle: a simply painted illustration of three al pastor tacos on a red plastic basket with wax paper, flat enamel colors, visible brush strokes. Below it, very large, yellow with a black outline: "3 for $6". Bottom, smaller black brush letters: "Tacos El Güero · Every Tuesday". No other text anywhere. Palette: white board, enamel red, yellow, black. Slightly uneven baselines, visible brush texture. No gradients, no photo elements, no sparkles.

### Wine bar tasting night (borrowed format: ticket)

> A vintage printed admission ticket, photographed flat from directly above on a dark green felt surface, landscape 3:2. The ticket is warm cream card with a perforated edge on the right side and a thin dark red border. Printed in dark red serif type: top line small caps "ADMIT ONE". Center, large: "NATURAL WINE NIGHT". Below: "Thursday 12 June, 7pm". Bottom left, small: "Vinoteca Prado". Bottom right, small: "$35". No other text anywhere. Slight letterpress impression and a subtle fold crease. No gradients, no glitter, no wine-glass clip art.

### What not to write

> ✗ "A stunning, vibrant, eye-catching poster for a bakery's weekend special with delicious pastries, modern and elegant design, high quality, 8k, professional."

Every word there is either generic or a hype word, so the model fills the gaps with its average: glossy pastries, swirls of steam, a script font and a gradient.
