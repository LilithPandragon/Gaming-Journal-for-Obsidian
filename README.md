# Game Journal (Obsidian)

A retro, notebook-style template for logging games you play, built for [Obsidian](https://obsidian.md/) with the [Templater](https://github.com/SilentVoid13/Templater) plugin and a matching CSS snippet.

![style](https://img.shields.io/badge/style-handwritten%20notebook-lavender)

## What's included

- **`Game Template.md`** - a Templater template. On creation it asks for the game's title, platform, and release year, then generates a note with:
  - Frontmatter (release year, platform, start/finish dates, completed/dropped flags, rating, tags)
  - **Why I wanted to play this**
  - **That one scene that thrilled / annoyed me**
  - **What I liked about it**
  - **In one sentence** - a quick table rating Graphics, Sound, Story, Gameplay, Controls, Difficulty
  - **My Rating** - a 10-box checklist that renders as a filled score (`x / 10`)
- **`Profile Template.md`** - a blank one-off "gamer profile" note (class, character stats, genre experience, equipment, first game ever played) plus a Dataview table that lists every game note, sorted by rating. This isn't a Templater template - it's a single file you fill in once by hand.
- **`gamejournal.css`** - a CSS snippet that gives notes with `cssclasses: gamejournal` a paper-and-ink, notebook look: bordered callout boxes, ruled writing lines, a pixel-style font for headers, and a clickable rating row.

## Installation

1. **Templater** (for `Game Template.md` only)
   - Install the *Templater* community plugin (Settings → Community plugins → Browse).
   - Copy `Game Template.md` into your configured Templater templates folder (e.g. `Templates/`).
   - In Templater's settings, set this as your default template for a "Games" folder, or trigger it manually via `Insert Template`.

2. **Profile note**
   - If you want you can also create a Profile of yours. Copy `Profile Template.md` directly into your gaming journal folder (e.g. `Games/`), not into the Templater templates folder - it's a normal note to fill in once, not something Templater runs.
   - Rename it, add your own profile picture if you like, and fill in the callouts.

3. **CSS snippet**
   - Copy `gamejournal.css` into `.obsidian/snippets/` in your vault.
   - Go to Settings → Appearance → CSS snippets and enable **gamejournal**.

4. **Dataview**
   - The profile note's game table needs the *Dataview* community plugin installed.

5. **Callouts**
   - Both notes use custom callout types (`game`, `scene`, `liked`, `sentence`, `rating`, `class`, `stats`, `genre`, `equipment`, `firstgame`, and optionally `screenshot`). No extra plugin is needed for these - Obsidian renders any `> [!name]` as a callout by default, and the CSS styles them by that name.

## Usage

1. Create a new note and run the Templater template (or set it as the default for a dedicated folder, e.g. `Games/`).
2. Enter the game title (the note is renamed automatically), pick a platform, and enter the release year.
3. Fill in the sections as you play. Check boxes in **My Rating** to build up your score out of 10.
4. Optionally fill in `Profile Template.md` once as your personal gamer profile - it doubles as an overview page since its table lists every note tagged `#game`.

## Customization

- **Platforms list**: edit the `platforms` array near the top of `Game Template.md`.
- **Colors/fonts**: all colors and the font stack are defined as CSS custom properties at the top of `gamejournal.css` (`--sj-ink`, `--sj-paper`, `--sj-lavender`, `--sj-line`, `--sj-pink`, `--sj-row`, `--sj-font`) - change them there to re-theme the whole journal.
- **Two-column reading view**: there's a commented-out block at the bottom of the CSS file to lay the note out in two columns in reading view, notebook-style.

## License

Feel free to use, modify, and share this.
