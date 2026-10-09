# Standalone game page

One page, no other site needed. `index.html` is the game (behind a password screen).

```
index.html                              the game (the song and sprites are inside it)
fonts/MS_Sans_Serif.ttf                 font for the password screen
media/final-video.mp4                   lyric video shown in the final spell
media/it-doesnt-end-here-lyrics.txt     OPTIONAL typed lyrics (see notes)
.nojekyll                               tells GitHub Pages to serve files as they are
```

## Put it online (GitHub Pages)

1. New repository on GitHub, set to Public.
2. Upload everything in this folder, keeping the folders. Drag in the *contents*, so `index.html` sits at the top level.
3. Settings > Pages > Deploy from a branch > `main` / `/ (root)` > Save.
4. After a minute the game is live at `https://USERNAME.github.io/REPO-NAME/`.

## Settings you may want (all near the top of the script in `index.html`)

- `GAME_PASSWORD`  the password (not case-sensitive)
- `START_LIVES`    lives at the start (currently 35)
- `FINAL_LIVES`    lives you get when the final spell begins (currently 20)
- `END_TITLE` / `END_SUB`  text on the stage-clear screen
- `TEST_PHASE_HP`  leave at 0. Any other number shrinks every phase before the final spell to that much health (testing only)

## Notes

- Keyboard only: arrows to move, Shift to focus, Z to shoot, X to bomb.
- The hi score only lasts until the page is refreshed or closed.
- The lyric video needs a browser that plays H.264 MP4 (Chrome, Edge, Safari and Firefox on normal installs do).
- `media/it-doesnt-end-here-lyrics.txt` is optional; without it the game just shows no typed lyrics.
