# Menu design and the layout route

Menus, price lists and schedules carry too much small text for the image tool to render reliably. Build them as a print-ready HTML file with Code Interpreter. Text is sharp at any size, prices are exactly right, and the owner can edit and reprint it.

## When to use the layout route

- More than about 20 words of text, or more than 4 text blocks.
- Any menu with more than a handful of items.
- Price lists, class timetables, opening hours for multiple locations.
- The real logo must appear exactly as supplied.
- Printing at A4 / US Letter or larger.

## Layout route workflow

1. Confirm all the text: sections, items, descriptions, prices, dietary marks, footer (address, hours, allergen note). Transcribe from an uploaded old menu if there is one.
2. If the direction needs artwork (a linocut illustration, a risograph shape, a photo), generate it first with the image tool, text-free: add "No text anywhere" to the prompt. Then save it to /mnt/data and embed it in the HTML as base64 so the file stays self-contained.
3. If the user uploaded a logo, embed it as base64 too.
4. Read menu-template.html from the knowledge files (in /mnt/data) and use it as the structure. Change the CSS variables, fonts, grid, rules and ornament to fit the chosen direction from style-directions.md. The template's default look is only a starting point.
5. Set the page size with `@page` (A4 `210mm 297mm`, Letter `8.5in 11in`, A3 `297mm 420mm`, tabloid `11in 17in`, or a custom size like a 4×9 in table card).
6. Save it as /mnt/data/<business>-<piece>.html and give the download link.
7. Give these print steps:
   > Open the file in Chrome or Edge → Print (Ctrl/Cmd+P) → Destination "Save as PDF" → Margins "None" → tick "Background graphics" → Save. Send that PDF to the printer, or print it yourself.
8. Say that fonts load from Google Fonts, so the computer opening the file must be online the first time.
9. For a screen version (Instagram, TV), offer a second HTML file sized in px (for example 1080×1350 or 1920×1080) that they can screenshot. You can also generate a version with the image tool if the text is short.

## Menu hierarchy

From strongest to weakest:
1. Business name or menu title (only if the menu isn't already in their space; often smaller than you'd think).
2. Section heads: Breakfast, Small plates, Drinks.
3. Item names.
4. Prices.
5. Descriptions.
6. Footer: dietary legend, allergen note, service charge, address, hours.

Make each level visibly different through size, weight, case or color, and use only one change per level. Don't use all four at once.

## Menu rules

- 5–7 items per section where possible. Long sections are split or put in two columns.
- Descriptions under 12 words, listing ingredients plainly (see copywriting.md).
- Prices: set right after the description or the name, same size or smaller, no currency symbol on sit-down menus, no ".00", no dot leaders. A right-aligned price column is fine for counter and takeaway menus, where speed matters more.
- Highlight at most one or two items per page (house special, new item) with a box, a color or an icon. Highlighting everything highlights nothing.
- Body text at least 9.5pt for printed table menus; dim bars and restaurants need 10.5–11pt.
- Wall and counter menus are read from 2–4 m away: item names at least 48–72pt equivalent, very short descriptions or none.
- TV menu boards: landscape, 1920×1080, at most 12–15 items per screen, high contrast, no thin type.
- Margins: at least 12mm on print. Leave room so a trim or a menu holder doesn't cut anything.
- One or two typefaces. Use the family's weights and italic before adding a second family.
- Dietary marks: one system, explained in a legend.

## Font pairings (Google Fonts) by direction

| Direction | Display | Text |
|---|---|---|
| Swiss grid | Archivo (700–900) | Archivo / Archivo Narrow |
| Risograph | Bricolage Grotesque | Space Mono or Bricolage Grotesque |
| Wood-type broadside | Big Shoulders Display | Zilla Slab |
| Hand-painted sign | Ultra / Yellowtail (one word only) | Work Sans |
| Bistro card | Libre Caslon Display | Libre Caslon Text or EB Garamond |
| Kissaten | Zen Maru Gothic | M PLUS Rounded 1c |
| Seventies | Fraunces (SOFT 100, WONK 1) | Karla |
| Bauhaus | Archivo Black | Archivo |
| Photocopy flyer | Anton | Courier Prime |
| Botanical plate | IM Fell English SC | IM Fell English |
| Linocut | Alfa Slab One | Zilla Slab |
| Grocery circular | Archivo Black | Archivo Narrow |
| Giant type | Instrument Serif or Bricolage Grotesque | Inter |

Avoid as defaults (they read as templates): Montserrat, Poppins, Raleway, Lobster, Pacifico, Great Vibes, Dancing Script, the Playfair Display + Montserrat combination, and Bebas Neue used for everything.

## Common menu formats

| Format | Size | Notes |
|---|---|---|
| Single-page table menu | A4 or US Letter | Most common. One or two columns |
| Long narrow card | 4×11 in / 99×210mm (DL) | Elegant for bistros and wine lists; one column |
| Folded menu | A3 or tabloid folded to A4/Letter | Make each half a separate page in the HTML |
| Table tent | A6 / 4×6 in, double-sided | Specials, drinks, QR code |
| Counter / wall menu | A2–A0 or custom | Huge type, few words |
| TV menu board | 1920×1080 px | Landscape, high contrast |
| Instagram menu post | 1080×1350 px | Few items, big type |
