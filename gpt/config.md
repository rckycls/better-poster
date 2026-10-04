# GPT builder settings

Values to paste into ChatGPT → Explore GPTs → **Create** → **Configure** tab. Creating a GPT needs a paid ChatGPT plan.

## Name

Better Poster

## Description

Posters, flyers and menus for small businesses that don't look like AI made them. Bring your text, a photo of your shop, and what it's for.

## Instructions

Paste the full contents of [`instructions.md`](instructions.md). It is about 6,100 characters; the builder's limit is 8,000.

## Conversation starters

1. Make a poster for my café's new weekend special
2. Redesign my menu (I'll upload a photo of the current one)
3. I need a flyer for an event at my shop
4. Turn this price list into something I can print

## Knowledge

Upload every file in [`knowledge/`](knowledge/):

- `anti-slop.md`
- `style-directions.md`
- `image-prompting.md`
- `menu-design.md`
- `copywriting.md`
- `menu-template.html`

## Capabilities

| Capability | Setting | Why |
|---|---|---|
| Image Generation | **On** | Image route: posters, flyers, social posts |
| Code Interpreter & Data Analysis | **On** | Layout route: builds print-ready HTML menus and reads `menu-template.html` |
| Web Search | Off | Not needed; tends to pull in generic references |
| Canvas | Optional | Handy for editing menu text together; not required |

## After publishing: test it

Try these and check the results against the checklist in `anti-slop.md`:

1. "Poster for Holm Bakery, cardamom buns Saturdays from 8am, 41 Dock St." It should ask at most one round of questions, offer 2–3 distinct directions, then produce a poster with every word spelled correctly.
2. Upload a photo of a real menu and say "make this better". It should transcribe the text, confirm it, choose the layout route, and give you a downloadable HTML file that prints to one page.
3. "Just make it pop." It should translate that into a concrete change and say what it changed.
4. "Make it look like a chalkboard with lots of swirls." It should do it, then offer one less generic alternative.
