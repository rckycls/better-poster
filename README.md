# better-poster

A Custom GPT for ChatGPT that designs posters, flyers and menus for small businesses (cafés, restaurants, salons, shops, venues) that don't look like generic AI output.

## How it avoids the generic AI look

- **Commits to a real design tradition** (risograph, wood-type broadside, hand-painted sign, Swiss grid, bistro card, linocut…) instead of the model's default glossy style, or lays the poster out as an everyday object (receipt, ticket stub, seed packet, timetable).
- **Uses the business's own stuff:** their products, colors from their shop, the way the owner talks.
- **Bans the tells:** floating ingredients, sparkles, gradients, faux chalkboards, script fonts, "indulge in a symphony of flavors", and the hype words in prompts ("stunning, vibrant, 8k") that cause them.
- **Gets the text right:** short pieces go through image generation with every word quoted and proofread; text-heavy menus become a print-ready HTML file (exact prices, real fonts, sharp at any size).
- **Checks before delivering,** using a 10-point checklist.

## Files

```
gpt/
  config.md              GPT builder settings: name, description, starters, capabilities, test prompts
  instructions.md        Paste into the "Instructions" field (under the 8,000-character limit)
  knowledge/             Upload all of these as Knowledge files
    anti-slop.md           Visual, copy and prompt clichés, plus the pre-delivery checklist
    style-directions.md    15 design directions, borrowed formats, business → direction map
    image-prompting.md     Prompt anatomy, text-rendering rules, sizes, example prompts
    menu-design.md         Menu hierarchy, font pairings, the HTML layout route
    copywriting.md         Headlines, menu descriptions, banned words
    menu-template.html     Print-ready A4 menu template used by the layout route
```

## Quickest way: no setup

Download [`better-poster.md`](better-poster.md), attach it to a new ChatGPT chat, and write "Follow this file. Here's what I need: …". It's a condensed one-file version of everything below. You'll need to attach it again in each new chat.

## Setup as a Custom GPT (one-time, then just click it)

1. In ChatGPT, open Explore GPTs → **Create** → **Configure**.
2. Fill in the fields from [`gpt/config.md`](gpt/config.md).
3. Paste [`gpt/instructions.md`](gpt/instructions.md) into **Instructions**.
4. Upload everything in [`gpt/knowledge/`](gpt/knowledge/) under **Knowledge**.
5. Turn on **Image Generation** and **Code Interpreter & Data Analysis**.
6. Run the test prompts at the bottom of `config.md`.

## Editing

- To add or change a style, edit `style-directions.md`. Keep its format (Good for / Type / Palette / Layout / Finish / Prompt fragment / Avoid) and add the style to the business map at the bottom of that file.
- When you change `instructions.md`, check the length stays under 8,000 characters: `wc -c gpt/instructions.md`.
- After editing knowledge files, re-upload them in the GPT builder and click **Update**.
