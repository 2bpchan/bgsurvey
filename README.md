# Board Game Tier Survey

An **offline**, single-file HTML tool for ranking board games on a tier list (S / A / B / C / D / F)
across three categories, then exporting the results as CSV.

## Use it

Just open **`index.html`** in any browser (double-click it — no server, no internet needed).

- Enter your name (optional), then tap a tier letter for each category on every game.
- **Categories:** Convenience (ease of setup/teardown + how easy it is to play while eating) · Overall Enjoyment.
- Tap a selected letter again to clear it.
- Everything auto-saves in the browser (localStorage), so you can close and come back.
- **Export CSV** downloads a spreadsheet: one row per game with columns
  `Rater, Date, Game, Convenience, Overall Enjoyment`.
- **Reset** clears all tier picks (your name stays).

## Images

Box art lives in **`images/<slug>.png`** and was pulled from BoardGameGeek. Games whose art
couldn't be auto-matched show a striped placeholder with the exact filename to add.

### To add a missing image manually
Find the game on BoardGameGeek, save its box image, and drop it into `images/` named exactly
as shown on the placeholder. Then reload `index.html`. (Any `<img>`-readable file works — the
extension can stay `.png` even if it's really a JPG.)

**Placeholders to fill in (ambiguous / not confidently matched):**

| Game | Expected file | Note |
|------|---------------|------|
| Daifugo | `images/daifugo.png` | traditional game, no single BGG box |
| Lumberjacks | `images/lumberjacks.png` | couldn't pin the exact title |
| Movies | `images/movies.png` | multiple BGG matches — pick yours |
| Gods | `images/gods.png` | multiple BGG matches — pick yours |
| Pirates | `images/pirates.png` | multiple BGG matches — pick yours |

If any auto-downloaded image turns out to be the wrong edition, just overwrite that
`images/<slug>.png` file.
