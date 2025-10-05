# Rialo — Car Avoid (Logo + Shield)

A **simple single-file HTML game** where you drive a car (logo) left and right to avoid obstacles falling from the top.  
Collect the **logo-coin** to activate a **Shield power-up** (6 seconds of invincibility) with a visual ring and countdown HUD.

> 🔗 **Live (GitHub Pages)**: Go to **Settings → Pages → Branch:** `main` → Save.  
> Once deployed, your game will be available at:
> ```
> https://<username>.github.io/<repo>/
> ```

---

## 🎮 Features
- **Single file**: Entire game inside `index.html` (HTML + CSS + JS)
- **Logo integration**: Your logo appears in the menu, player car, HUD, and shield coin.
- **Shield power-up**: Collect logo coin for a 6-second invincibility shield (with ring + countdown).
- **Dynamic difficulty**: Speed and obstacle frequency increase over time.
- **Best score tracking**: Saved in `localStorage`.
- **Mobile friendly**: Includes on-screen touch buttons.

---

## ⌨️ Controls
- **Start / Pause** — Button or **Enter** key  
- **Move** — **← →** or **A / D**  
- **Restart** — **R**

---

## 🛠️ Run Locally
1. Download or clone this repository.
2. Double-click `index.html` to open the game in your browser.  
   Or use a simple local server:
   ```bash
   # Python 3
   python -m http.server 8000
   # Then open http://localhost:8000/index.html
   ```

---

## 🚀 Deploy (GitHub Pages)
1. Commit and push your `index.html` file to this repo.  
2. Go to **Settings → Pages → Branch:** `main`, then click **Save**.  
3. After a few minutes, your live game will appear at:
   ```
   https://<username>.github.io/<repo>/
   ```

---

## 🗂️ Project Structure
```
repo/
└─ index.html   # Full game source (HTML + CSS + JS)
```
> Note: This version includes the logo as an **embedded data URL**, so you don’t need any separate image files.

---

## 🧩 Customization
- **Change logo** — replace the data URL or edit `logo.src` inside `index.html`
- **Number of lanes** — change the `lanes` variable (default = 3)
- **Shield duration** — adjust in `activateShield(6000)` (milliseconds)
- **Speed/difficulty** — tweak `speed`, `diffMult`, and `spawnEvery`
- **Color theme** — edit CSS `:root` variables (`--bg`, `--road`, `--lane`, `--accent`, `--good`, etc.)

---

## 🤝 Contributions
Pull requests are welcome!  
Open an Issue for bugs, ideas, or improvements.

---

## 📜 License
**MIT License** — Use freely at your own risk.  
(Logo ownership and usage rights remain with the creator.)
