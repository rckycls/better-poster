# Anti-slop guide

"AI slop" is work that's technically fine but generic: it could belong to any business, it uses the default look the model reaches for, and people scroll past it because they've seen it a thousand times. This file lists the tells and what to do instead. Re-read it before every generation.

## The core test

Cover the business name. Could this poster belong to any other café, salon or pizza place? If yes, it's slop. Fix it by adding something only this business has: their product, their street, their colors, their way of talking, their actual opening hours.

## Visual tells → what to do instead

| Tell | Instead |
|---|---|
| Glossy, over-rendered 3D look, plastic surfaces | Flat print processes (screen print, risograph, letterpress, linocut) or honest photography |
| Teal-and-orange or purple-blue gradient grading | 2–4 flat colors taken from the business (awning, tiles, cups, packaging) |
| Ingredients floating, splashing or exploding around the product | One product, sitting on a real surface, photographed or drawn plainly |
| Steam swirls, sparkles, glitter, lens flares, light rays, bokeh | Nothing. Let the product and the type carry it |
| Everything centered and symmetrical, by default | A grid: flush-left type, an off-center focal point, deliberate empty space |
| Every corner filled with decoration, ribbons, banners, badges | One focal point, one headline, small supporting info. Empty space is part of the design |
| Fake chalkboard, wood-plank or kraft-paper backgrounds | Real materials only if the business has them; otherwise a flat paper color |
| Generic fonts: rounded geometric sans, Playfair + Montserrat, curly scripts | Type chosen for the direction (see menu-design.md); condensed grotesques, slab serifs, wood type, honest serifs |
| Drop shadows, outer glows, bevels and outlines on text | Contrast through size, weight and color, not effects |
| Perfect smiling stock-photo people | No people, or candid ones: hands at work, a back turned, a crowd at night |
| "Delicious food" in general | Their actual dish, named, plated how they serve it |
| Clip-art icons (coffee cup with heart steam, scissors, dumbbell) | A specific object drawn or photographed with character, or no icon |
| Gibberish text, fake words in the background | "No other text" in every prompt; check the result |
| Ornamental swirls, flourishes, laurel wreaths around everything | One rule line or one small mark, if anything |
| Neon glow on everything for anything "night" | Black paper with one fluorescent ink, or a flash photo |
| Over-saturated "vibrant" colors | Real ink colors: muted, slightly off, on paper |

## Composition tells

- Headline, image and info all about the same size. Make the headline at least 3× the body text, or make the image dominate and the text small.
- Headline sitting in a ribbon or banner shape. Set it straight on the paper.
- Text running over a busy photo with a shadow to make it readable. Give the text its own space.
- Five different fonts. Use one family or two, never three.
- Every element given equal margins like a template. Let something bleed off the edge, or crop the product hard.

## Copy tells

See copywriting.md for the full list. Biggest offenders: "Elevate", "Indulge", "Experience", "Discover", "Unleash", "journey", "symphony of flavors", "where X meets Y", "crafted with love", "taste the difference", "your new favorite", "a feast for the senses", exclamation marks everywhere, emojis.

## Prompt words that produce slop

Never put these in an image prompt: stunning, beautiful, gorgeous, vibrant, eye-catching, high quality, best quality, masterpiece, professional, ultra detailed, hyperrealistic, photorealistic, 4k, 8k, cinematic, epic, dramatic lighting, award-winning, trending, modern and sleek, elegant, luxurious, premium, sophisticated, clean design.

They push the model toward its average, over-polished look. Replace each with a physical, specific description:
- "premium" → "uncoated cream stock, one dark green ink, lots of margin, small serif type"
- "modern" → "flush-left condensed grotesque on a strict 6-column grid, one accent color"
- "vibrant" → "fluorescent pink and blue risograph inks on white paper"
- "professional photo" → "shot on 35mm film with direct on-camera flash, slightly overexposed"
- "elegant" → "thin rules, small caps, wide letterspacing, centered on a narrow column"

## Pre-delivery checklist

Before showing anything, check all of these. Fix any failures first.

1. **Specific:** something in it could only belong to this business (product, place, color, phrase).
2. **One focal point:** you can say in four words what the eye hits first.
3. **Hierarchy:** headline clearly dominates, and supporting info is grouped and small.
4. **Palette:** 2–4 colors, and you can name where each one came from.
5. **Type:** at most two families, chosen for the direction, with no effects.
6. **Text accuracy:** every word spelled correctly; prices, dates, times and addresses match the brief exactly; no invented facts; no gibberish.
7. **Copy:** no banned words, no emojis, at most one exclamation mark.
8. **Fit:** readable at the real viewing distance (window poster from 3 m, phone screen, table menu at arm's length).
9. **Direction:** it looks like the chosen direction, not like a generic "nice poster".
10. **Restraint:** remove one more thing. Is it better? Then leave it out.
