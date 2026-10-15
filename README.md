# Tapeline

**Free floor plan sketching for appraisers.** Draw exterior outlines by typing measurements, get square footage and totals instantly, and export a clean picture for your report. It is one file that runs in your web browser. Nothing to install, nothing to buy, and nothing you draw is ever sent anywhere.

- **Use it online:** https://joshthomdan.github.io/tapeline/
- **Download it (one file):** https://github.com/joshthomdan/tapeline/releases/latest/download/tapeline.html

Tapeline works best on a computer with a keyboard and mouse (Windows or Mac). It runs in Chrome, Edge, Firefox and Safari.

> Please read the [Disclaimer](DISCLAIMER.md). Tapeline was built with the help of AI and is provided as is, with no warranty. You are responsible for checking every measurement and total before you use it in an appraisal or report.

---

## What it does

- **Keyboard drawing.** Type a distance and press an arrow key. Moves add up into one wall until you press Enter, so `3 Down 3 Right Enter` draws one 45 degree wall. Press **A** to close the outline.
- **Mouse drawing** with snapping to corners, walls and line-ups, if you prefer.
- **Square footage and totals** calculated from the walls, always. Living Area Total, plus separate totals for garages, basements and other categories.
- **Areas inside other areas** (for example a garage drawn inside the house outline): it asks whether to subtract, and remembers your answer.
- **Final Check** lists open outlines, areas without a category, overlaps and unanswered questions before you export.
- **Room labels, free text, stairs and doors.** Doors snap onto walls.
- **Edit a wall's length** after drawing; the shape stays square.
- **Copy, paste, rotate, mirror, duplicate** (for example to make a second floor from the first).
- **Undo and Redo** (250 steps).
- **Save and open project files** (`.sketch.json`), automatic recovery copies in your browser, and **PNG or JPEG export**.
- **Built-in self-tests**: 107 automatic checks you can run any time from the toolbar.

## Quick start

1. Open the program (online link above, or double-click the downloaded file).
2. Click **Load Example** to see a finished sample house, or **New Project** to start fresh.
3. Press **F4** (or **N**, handy on a Mac) to start an area. Pick a category such as First Floor and press **Enter**.
4. Click where the first corner goes, or just press **Enter**.
5. Type the walls: `40` then the **Right arrow**, then **Enter**. Then `30` **Down**, **Enter**. Then `40` **Left**, **Enter**. Press **A** to close. You now have 1,200.0 sf.
6. Click **Final Check**, then **Export Image** to save a picture for your report.
7. Click **Save** to keep a project file you can open again later.

Click **Help** inside the program for every shortcut. On a Mac, use Command wherever it says Ctrl.

## Your data

Tapeline makes no internet connections. Your sketches live only in the files you save. Recovery copies are kept in your own browser as a safety net; they are not a backup, so always save a project file.

## Browser notes

| Browser | Notes |
|---|---|
| Chrome, Edge | Everything works, including saving straight back to the same file. |
| Firefox, Safari | Everything works. **Save** downloads a copy to your Downloads folder instead of overwriting the file. **Copy Image** may be blocked; **Export Image** always works. |
| Phones and tablets | You can look at a sketch, but drawing needs a keyboard. Open the link on your computer. |

---

## How to customize this with AI

Tapeline is a single file written so that people with no coding background can ask an AI (such as Claude or ChatGPT) to change it. You are free to change it and share your version (see the License).

### Before you start

1. **Keep a copy of the file that works.** Name it something like `tapeline-original.html`.
2. Know where things are. Open the file in any text editor (Notepad on Windows, TextEdit on a Mac). Near the top is **PART A. SETTINGS YOU CAN CHANGE**. It holds:
   - the program name and colors
   - the room label list
   - the area categories (First Floor, Garage and so on) and which ones count toward living area
   - the levels
   - the default settings
   - the image formats for Export Image
   - the stairs and door symbols, and how each one is drawn

### Small changes (labels, colors, categories)

You can make these yourself in Part A with a text editor: change the words between the quote marks, keep the commas, save, and reopen the file. Or copy just Part A into an AI chat, ask for the change, and paste the result back in place of the old Part A.

### Bigger changes (a new feature)

The file is large (about 400 KB). Some chat windows cannot read or send back a file that size in one piece. The most reliable way is an AI tool that can open and edit files on your computer directly (for example the Code feature in the Claude desktop app). In a regular chat, attach the file and ask for exact "find this text, replace it with this text" changes.

**Example prompt you can paste:**

```
I am attaching tapeline.html, a free floor plan sketching program for real estate
appraisers. It is one self-contained HTML file. Please add a new symbol called
"Fireplace": a rectangle 5 ft wide and 2 ft deep with a smaller rectangle inside it,
placed and moved like the other symbols.

Rules:
1. Keep it ONE self-contained HTML file. No outside files, libraries, fonts or
   internet connections.
2. Make the change in "PART A. SETTINGS YOU CAN CHANGE" if possible, following the
   pattern of the existing symbols. Do not rename the existing symbol codes.
3. Do not change how walls, areas, square footage or totals are calculated.
4. Add a self-test for the new feature in section 7 if it makes sense, and keep all
   existing self-tests passing.
5. Keep the plain-English comments up to date, and use plain language in anything
   people will see on screen.
6. Tell me in plain language exactly what you changed.
```

Other ideas you can swap in for the first paragraph:

- "Add 'Sunroom' and 'Bonus Room' to the room labels, and add an area category called 'Screened Porch' that does not count toward living area."
- "Add a spiral staircase symbol: a circle with lines from the center like spokes and an arrow."
- "Add WEBP as an Export Image option."
- "Change the wall color to black and make the lettering a little larger by default."

### After any change

1. Open the changed file in your browser.
2. Click **Run Self-Tests** on the toolbar. Every test should say **PASS**. If any say FAIL, give the AI the test number and the details shown, and ask it to fix the problem.
3. Click **Load Example** and try the new feature by hand.
4. Draw a shape you know the answer to (for example a 40 by 30 rectangle is 1,200.0 sf) and check the total.
5. If the program shows "The program could not start," go back to your working copy, or give that message to the AI.

---

## Known limits

- Arrow-key drawing goes straight up, down, left and right on the page. Draw an area first, then rotate it.
- Copy and paste work inside one browser window only.
- Recovery copies stay in the browser where they were made.
- Square footage is shown to one decimal place. Totals are added up before rounding, so a total can differ by 0.1 sf from adding up the rounded labels.
- Tapeline does not decide what counts as gross living area and does not apply any measuring standard. Those decisions are yours.

## Files in this project

| File | What it is |
|---|---|
| `tapeline.html` | The whole program. This is the only file you need to use it. |
| `index.html` | A tiny page that sends web visitors to `tapeline.html`, so the web address stays short. |
| `README.md` | This page. |
| `DISCLAIMER.md` | The full disclaimer. Please read it. |
| `LICENSE` | The MIT License. |

## Disclaimer (short version)

This program was built with the help of artificial intelligence. I have found it accurate in my own use, but it is provided as is, with no warranty of any kind. Users are solely responsible for verifying all measurements, calculations and sketches before relying on them in any appraisal or report. I am not responsible for any errors, losses or damages arising from its use. It is not affiliated with or endorsed by any commercial software company or by the Appraisal Institute. Full text: [DISCLAIMER.md](DISCLAIMER.md).

## License

Free and open source under the [MIT License](LICENSE). Copyright (c) 2026 Joshua Daniel. You may use, copy, change and share it, including your changed versions, as long as the license notice stays with it.
