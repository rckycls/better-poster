# Better Poster

**Better posters, flyers and menus for small businesses, made with ChatGPT, without the "AI look".**

Cafés, restaurants, food trucks, bakeries, salons, shops, gyms, venues: tell it what you need and it designs something that looks like a real designer made it for *your* business, not a glossy, sparkly, generic AI picture.

You don't need to know anything about design, coding or GitHub. Pick one of the methods below and follow the steps.

---

## Which method should I use?

| Method | Setup time | Free ChatGPT? | Remembers next time? | Best for |
|---|---|---|---|---|
| [**A. Paste a link**](#method-a-paste-a-link-fastest) | None | ✅ | ❌ paste again each chat | Trying it right now |
| [**B. Attach the file**](#method-b-attach-the-file) | 1 minute | ✅ (upload limits apply) | ❌ attach again each chat | Most reliable quick option |
| [**C. Copy and paste the text**](#method-c-copy-and-paste-the-text) | 1 minute | ✅ | ❌ paste again each chat | When links and uploads don't work |
| [**D. ChatGPT Project**](#method-d-chatgpt-project-set-up-once) | 3 minutes | ✅ if your plan has Projects | ✅ | Using it regularly |
| [**E. Custom GPT**](#method-e-custom-gpt-best-results) | 5 minutes | ❌ needs a paid plan to create | ✅ | Best results; sharing with others |

**Not sure?** Start with **A**. If you end up using it every week, set up **D** or **E** once and never think about it again.

> ChatGPT changes its plans and menus often. If a button has moved or a feature is missing on your plan, just try the next method.

---

## Method A: Paste a link (fastest)

No downloads, no setup.

1. Go to **[chatgpt.com](https://chatgpt.com)** (or open the ChatGPT app) and start a **new chat**.
2. Copy this whole message, paste it into the chat, and replace the last line with what you need:

   ```
   Read the full file at https://raw.githubusercontent.com/rckycls/better-poster/main/better-poster.md and follow it as your instructions for this whole chat.

   Here's what I need: a poster for my bakery. Cardamom buns, Saturdays from 8am, 41 Dock St.
   ```

3. Press send. ChatGPT reads the file and asks you a few quick questions about your business.

**If it says it can't open the link**, or it seems to ignore the instructions, use Method B or C instead. Reading links needs ChatGPT's web search to be working.

---

## Method B: Attach the file

The most reliable quick option.

1. **Download the file:**
   - Open **[better-poster.md](better-poster.md)** on GitHub.
   - Click the **download icon** (an arrow pointing down, near the top right of the file).
   - It saves to your Downloads folder as `better-poster.md`.
2. Go to **[chatgpt.com](https://chatgpt.com)** and start a **new chat**.
3. **Attach the file:** click the **+** or 📎 (paperclip) button next to the message box and choose `better-poster.md`, or drag the file into the chat window.
4. Type your request and send:

   ```
   Follow this file as your instructions for this whole chat.

   Here's what I need: a poster for my bakery. Cardamom buns, Saturdays from 8am, 41 Dock St.
   ```

**On a phone:** download the file first (it goes to your Files app), then in the ChatGPT app tap **+** → **Files** and pick it.

---

## Method C: Copy and paste the text

Works even if you can't upload files and the link doesn't work.

1. Open the **[raw text of the file](https://raw.githubusercontent.com/rckycls/better-poster/main/better-poster.md)**.
2. Select everything (**Ctrl+A** on Windows, **Cmd+A** on Mac, or long-press and **Select all** on a phone) and copy it (**Ctrl+C** / **Cmd+C**).
3. Go to **[chatgpt.com](https://chatgpt.com)**, start a **new chat**, and paste it (**Ctrl+V** / **Cmd+V**).
4. On a new line under the pasted text, write what you need, for example: `Here's what I need: a poster for my bakery…`
5. Press send.

---

## Method D: ChatGPT Project (set up once)

A Project is a folder in ChatGPT with its own instructions. Every chat you start inside it follows the Better Poster rules automatically, with nothing to paste.

**Set it up (once):**
1. Download `better-poster.md` (see [Method B, step 1](#method-b-attach-the-file)).
2. In ChatGPT's left sidebar, click **Projects** → **New project**. Name it `Better Poster`.
3. Open the project and find **Instructions**. You may need to click the project's **⋯** menu or settings icon.
4. Paste this into the instructions box and save:

   ```
   You are Better Poster. Follow the attached file better-poster.md exactly, in every chat in this project. It contains your workflow, design rules and checklist.
   ```

5. Find **Files** (or **Add files**) in the project and upload `better-poster.md`.

**Use it:** open the **Better Poster** project from the sidebar and start a chat inside it. Just say what you need, e.g. "Menu for my taco truck", and attach a photo of your truck or old menu if you have one.

---

## Method E: Custom GPT (best results)

This gives you your own "Better Poster" app inside ChatGPT, using the full set of files: more styles, more examples, and a ready-made menu template. Creating it needs a **paid ChatGPT plan** (Plus, Pro, Team or Enterprise), and you need to do it on a **computer**. Once it's made, anyone you share it with can use it, including on the phone app.

**Step 1: Download the files**
1. Click this link: **[Download all files (ZIP)](https://github.com/rckycls/better-poster/archive/refs/heads/main.zip)**
2. Find the ZIP in your Downloads folder and **unzip** it (double-click on Mac; on Windows, right-click → **Extract All**).
3. Open the unzipped folder, then open the `gpt` folder inside it.

**Step 2: Create the GPT**
1. Go to **[chatgpt.com/gpts/editor](https://chatgpt.com/gpts/editor)**, or in ChatGPT click **GPTs** in the sidebar → **+ Create**.
2. Click the **Configure** tab at the top. Ignore the "Create" tab.
3. Fill in the boxes:

   | Box | What to put |
   |---|---|
   | **Name** | `Better Poster` |
   | **Description** | `Posters, flyers and menus for small businesses that don't look like AI made them. Bring your text, a photo of your shop, and what it's for.` |
   | **Instructions** | Open `gpt/instructions.md` with Notepad (Windows) or TextEdit (Mac), select all, copy, and paste it here. |
   | **Conversation starters** | Add these four, one per box: `Make a poster for my café's new weekend special` · `Redesign my menu (I'll upload a photo of the current one)` · `I need a flyer for an event at my shop` · `Turn this price list into something I can print` |

4. Under **Knowledge**, click **Upload files** and select **all 6 files** in the `gpt/knowledge` folder.
5. Under **Capabilities**, tick **Image Generation** and **Code Interpreter & Data Analysis**.
6. Click **Create** (top right) → choose **Only me** (or **Anyone with the link** to share it) → **Save**.

**Use it:** click **Better Poster** in your ChatGPT sidebar, or type `@Better Poster` in any chat to bring it in.

---

## Using it: what to say

You don't need special wording. Just tell it what you need like you'd tell a friend who designs. These help a lot:

- **What it's for:** a menu, a sale, an event, an opening, new hours, hiring.
- **Where it goes:** shop window, counter, table, Instagram post, Instagram story, TV screen, A4 or Letter print.
- **The exact words and prices.** It will never make up prices or dates; if you leave them out, it puts in `[PRICE]` for you to fill.
- **📷 A photo of your shop, products or old menu.** This is the best way to make the design feel like *yours*.

**Example requests:**
- "Poster for my taqueria's Taco Tuesday: 3 tacos for $6, every Tuesday. It goes in the window."
- "Here's a photo of my current menu. Make it look better, same prices. We're a cozy wine bar."
- "Instagram story for my salon: 20% off color treatments, 1–15 March. Our salon is all green velvet and brass."
- "Flyer for a live jazz night at my café, Thursday 12 June 8pm, free entry."

**After the first design:** ask for specific changes ("bigger headline", "use our green", "make a story version too"). It changes one thing at a time and keeps the rest.

---

## Printing a menu

For menus and price lists, Better Poster makes a **print-ready file** (ending in `.html`) instead of a picture, so every price is exact and the text stays sharp.

1. Click the **download link** ChatGPT gives you.
2. Open the downloaded file. It opens in your web browser; **Chrome** or **Edge** works best.
3. Press **Ctrl+P** (Windows) or **Cmd+P** (Mac).
4. Set:
   - **Destination:** Save as PDF
   - **Margins:** None (under "More settings")
   - **Background graphics:** ✅ ticked
5. Click **Save**. Print that PDF, or send it to a print shop.

**No download link?** Some plans can't create files. Ask ChatGPT: *"Give me the full HTML in one code block"*, then:
- **Windows:** open **Notepad**, paste, **File → Save as**, set "Save as type" to **All files**, and name it `menu.html`.
- **Mac:** open **TextEdit**, go to **Format → Make Plain Text**, paste, then save as `menu.html`.

Then follow the printing steps above.

---

## Troubleshooting

| Problem | Fix |
|---|---|
| It "can't open the link" | Use Method B (attach) or Method C (paste). |
| It's ignoring the rules or the designs look generic again | Say: *"Re-read the Better Poster instructions and follow them strictly."* Long chats drift, so start a new chat if needed. |
| A word or price is misspelled in the image | Say: *"Fix the spelling of [word], keep everything else exactly the same."* For lots of text, ask for the menu (HTML) version instead. |
| My logo came out wrong | Image tools redraw logos. Ask it to leave a blank space for the logo, or to make the HTML version with your logo file inserted exactly. |
| The image is blurry when printed big | Pictures from ChatGPT are about 1024×1536 pixels, fine up to about A5 / half-letter. For bigger prints, ask for the HTML version. |
| "You've reached the limit" for images or uploads | That's your ChatGPT plan's limit. Wait for it to reset, or use Method C (paste) to avoid uploads. |
| I can't find "Projects" or "Create a GPT" | Your plan may not include them. Use Method A, B or C. |

---

## How it avoids the AI look

- **Commits to a real design style** (risograph, wood-type poster, hand-painted sign, Swiss grid, bistro card, linocut…) instead of the default glossy AI look, or lays the poster out like an everyday object (receipt, ticket stub, seed packet, timetable).
- **Uses your business's own stuff:** your products, colors from your shop, the way you talk.
- **Bans the tells:** floating ingredients, sparkles, gradients, fake chalkboards, curly fonts, "indulge in a symphony of flavors", and the hype words ("stunning, vibrant, 8k") that cause them.
- **Gets the text right:** short posters are generated with every word checked; text-heavy menus become a print-ready file with exact prices.
- **Checks its own work** against a 10-point checklist before showing you.

---

## For maintainers

### Files

```
better-poster.md         One-file version (Methods A–D): condensed instructions + rules
gpt/                     Full version (Method E: Custom GPT)
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

### Editing

- **Two versions:** `better-poster.md` is a condensed copy of `gpt/`. When you change a rule or style in one, update the other.
- To add or change a style, edit `gpt/knowledge/style-directions.md`. Keep its format (Good for / Type / Palette / Layout / Finish / Prompt fragment / Avoid), add the style to the business map at the bottom, and add a one-line version to `better-poster.md`.
- Keep `gpt/instructions.md` under 8,000 characters: `wc -c gpt/instructions.md`.
- After editing knowledge files, re-upload them in the GPT builder and click **Update**.
