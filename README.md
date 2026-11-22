# SudokuVerse - Infinite Puzzle Challenge

**GamerKie Edition**

A standalone HTML5 Sudoku game. The game has no external JavaScript or CSS dependencies.

## Included in this build

- Seven difficulty selections: Easy, Medium, Hard, Very Hard, Expert, Master and Extreme.
- Procedurally generated 9x9 Sudoku puzzles. Clues are removed only when the puzzle still has exactly one solution.
- Independent level progression for each difficulty.
- Daily puzzle generated from the player's local date.
- 81-cell interactive board with row, column, box and matching-number highlights.
- Number pad, pencil notes, auto-candidates, erase, undo, redo, hint and check.
- Timer, mistake limits, pause/resume and restart.
- Local progress saving, statistics, achievements, personal records and JSON backup import/export.
- Five themes and responsive desktop/mobile layout.
- Desktop keyboard controls: 1-9, arrow keys, Delete/Backspace, N, H, U, R and Escape.

## Run locally

Open `index.html` in a modern browser. For the most reliable save behavior, serve the file from a local web server or deploy it to a static host. Progress is stored in browser LocalStorage for that origin.

## Deploy to GitHub Pages

1. Create a GitHub repository, for example `sudokuverse`.
2. Upload `index.html` to the repository root.
3. Open **Settings -> Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select the `main` branch and `/ (root)`, then save.
6. Open the Pages URL shown by GitHub, typically `https://YOUR-USERNAME.github.io/sudokuverse/`.

## Embed in Blogger

After GitHub Pages is published, paste this into a Blogger post using the HTML view. Replace the example URL with your actual Pages URL.

```html
<div style="width:100%;max-width:1100px;margin:0 auto;">
  <iframe
    src="https://YOUR-USERNAME.github.io/sudokuverse/"
    title="SudokuVerse - GamerKie Sudoku Game"
    loading="lazy"
    allow="fullscreen"
    style="display:block;width:100%;height:1000px;border:0;border-radius:14px;">
  </iframe>
</div>
```

## Honest scope notes

This is a working, offline-first single-player edition. Personal records and achievements are saved on the current browser/device; there is no online account system or real global leaderboard. The seven difficulty choices use progressively lower clue targets while preserving unique solutions, but the generator does not yet implement a full human-technique difficulty grader or every specialist strategy named in the original design brief (for example Swordfish, XY-Wing, forcing chains and coloring). Countdown Time Attack, cloud sync, music tracks and online rankings are not included in this build.

Daily puzzle generation uses the player's local calendar date and a fixed generator version. Clearing browser storage or changing browser/device will not sync progress; export a JSON backup before resetting or moving devices.
