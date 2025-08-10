# Cemong Helper — Gamer Edition (v1.4.1)
A lightweight helper for **Cabal Knight** focused on **Auto Loot** with a clean dark UI, compact overlay, and one-file build.

> **Download:** go to **Releases →** [latest](https://github.com/Acehgabana/Cemong-Helper/releases/latest)

---

## ✨ Features
- **Auto Loot** (default key: **F9**)  
  - Speed presets: **Fast (0.3s)**, **Normal (0.7s)**, **Slow (1.0s)**
  - Runs only when **Cabal Knight** window is active
- **Overlay** (drag-able, auto-hides when game not active)  
  - Shows **Status (ON/OFF)** and **Speed**
- **Modern Dark UI** with round logo link buttons (Website & Discord)
- **Single-file friendly**: assets (icon/tagline/logos) can be embedded
- **Versioned title**: `Cemong Helper v1.4.1 — Gamer Edition`

---

## 📥 Download & Run (End-users)
1. Download `Cemong Helper v1.4.1.exe` from **Releases →** [latest](https://github.com/Acehgabana/Cemong-Helper/releases/latest)
2. In-game, set **Hotkey 1 = F9** (Game → `O` → Key Bindings → Battle and Option → Hotkey 1).

---

## 🧰 Build from Source (Developers)
Tested on **Windows 11 / Python 3.11–3.13**.

### 1) Install requirements
```
pip install -r requirements.txt
```

### 2) Build (PyInstaller)
```powershell
pyinstaller --onefile --noconsole --icon "cemong.ico" "cemong_helper_v1_4_1_title_fixed.py"
```
Output: `dist\Cemong Helper v1.4.1.exe`

### 3) Optional: Smaller EXE with UPX
- Download UPX → extract to `C:\UPX\`
```powershell
pyinstaller --onefile --noconsole --clean --icon "cemong.ico" --upx-dir "C:\UPX" "cemong_helper_v1_4_1_title_fixed.py"
"C:\UPX\upx.exe" --best --lzma ".\dist\Cemong Helper v1.4.1.exe"
```

---

## ⚙️ Configuration
Edit the code to set your official URLs:
```python
CABAL_WEBSITE_URL = "https://github.com/Acehgabana/Cemong-Helper"
CABAL_DISCORD_URL = "https://discord.gg/<your_invite>"
```

---

## 📝 Changelog
### v1.4.1
- Fixed window title to match `VERSION = "1.4.1"`
- Links section with **round 32×32 logos** + accent ring
- Overlay shows **Status** and **Speed**
- Auto Loot speeds: **0.3s / 0.7s / 1.0s**
- Embedded assets support (icon, tagline, logos)

---

## 📄 License
MIT
