# Border Control NZ

A satirical browser game about New Zealand's cruel animal import loophole.

**Play it now:** [https://rubencastaing.github.io/border-control-nz/border-control-nz.html](https://rubencastaing.github.io/border-control-nz/border-control-nz.html)

---

## What is this?

New Zealand has banned cruel farming practices like battery cages and sow stalls domestically — but still allows imports of products made using those exact same practices overseas.

This game lets you be the border inspector NZ should have, but doesn't. Guide the Luxon Ostrich into cruel imports to block them before they cross the border!

The game is 99% LLM written.

---

## Files in this Projects

| File | What it is |
|------|-----------|
| `border-control-nz.html` | The game itself (everything is in this one file) |
| `Ostrich.png` | The character image |
| `Chris_luxon.webp` | Placeholder politician image |
| `Background_music.mp3` | Background music that plays during the game |
| `Animal_sounds.mp4` | Farm animal sounds that play as ambient noise |

---

## How to Run Locally

If you want to run the game on your own computer instead of using the online link:

### Option 1: Just open the file
Double-click `border-control-nz.html` to open it in your browser. The game will work, but audio files won't load (browsers block local file audio for security reasons).

### Option 2: Run a local server (for full audio)

#### On Mac / Linux
1. Open **Terminal**
2. Navigate to the folder containing the game files:
   ```
   cd /path/to/your/folder
   ```
3. Start a simple server:
   ```
   python3 -m http.server 8000
   ```
4. Open your browser and go to: **http://localhost:8000/border-control-nz.html**

#### On Windows
1. First, check if you have Python installed: open **Command Prompt** (search "cmd" in the Start menu) and type `python --version`. If you see a version number, you're good!
2. If you don't have Python, download it from [python.org](https://www.python.org/downloads/) — during install, **tick the box that says "Add Python to PATH"** (this is important!)
3. Open **Command Prompt** and navigate to the game folder. For example, if it's on your Desktop:
   ```
   cd %USERPROFILE%\Desktop\Animal_welfare_game
   ```
4. Start the server (note: on Windows it's `python` not `python3`):
   ```
   python -m http.server 8000
   ```
5. Open your browser and go to: **http://localhost:8000/border-control-nz.html**
6. To stop the server when you're done, press **Ctrl+C** in the Command Prompt window

---

## How to Update the Game

If you want to change something (like the campaign URL, facts, or text):

1. Open `border-control-nz.html` in any text editor
2. Search for `CAMPAIGN_URL` to find the campaign link — change it to your real URL
3. Search for `GAME_URL` to update the sharing link
4. Search for `FACT: UPDATE THIS` to find all the facts and statistics you can edit
5. Save the file

---

## Adding Sound Effects (Optional)

The game supports optional sound effect files. If you add any of these files to the same folder, they'll play automatically:

| File name | When it plays |
|-----------|--------------|
| `sfx_start.mp3` | When the game starts |
| `sfx_gameover.mp3` | When the game ends |
| `marmite_splat.mp3` | When you block a cruel product |
| `sfx_wrong.mp3` | When you accidentally block a safe product |
| `luxon_ostrich.mp3` | When the character is in Stage 0 (head in sand) |
| `luxon_peek.mp3` | When the character reaches Stage 1 (peeking) |
| `luxon_stand.mp3` | When the character reaches Stage 2 (standing) |
| `luxon_hero.mp3` | When the character reaches Stage 3 (hero mode) |
| `luxon_fail.mp3` | When the character regresses a level |

If these files are missing, the game falls back to synthesised sounds — so it works fine without them.

---

## Embedding on a Website

To embed the game on a WordPress site or any other website, use an iframe:

```html
<iframe src="https://rubencastaing.github.io/border-control-nz/border-control-nz.html"
        width="100%" height="800" style="border:none; max-width:600px;"
        allow="autoplay"></iframe>
```

---
