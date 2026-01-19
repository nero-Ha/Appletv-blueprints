# 📺 Appletv-blueprints

Home Assistant blueprints for **Apple TV**, **Chromecast**, and **Movie Mode** automations.

A small collection of clean, reusable blueprints focused on media-based lighting and cover control.

---

## 🎬 Quick Import of Blueprints

You can import the following blueprints directly into your Home Assistant instance by clicking the buttons below:

| Blueprint | Description | Import |
|-----------|-------------|--------|
| **Play Detection** | Detects when Apple TV or Chromecast starts playing media and turns ON Movie Mode | [![Import](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?url=https://gist.githubusercontent.com/nero-Ha/89c419fad7593fd07a82958e88249e3d/raw/movie_mode_save_restore.yaml) |
| **Stop / Pause Detection** | Detects when media is paused or stopped and turns OFF Movie Mode | [![Import](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?url=https://gist.githubusercontent.com/nero-Ha/7d25335bf65c94c4c428ace105856a81/raw) |
| **Lights & Covers Snapshot / Restore** | Saves the current state of lights and covers, closes covers on Movie Mode start, and restores them after Movie Mode ends | [![Import](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?url=https://gist.githubusercontent.com/nero-Ha/e6379e81975b4606fa520f24b82e46b2/raw/movie_mode_save_restore.yaml) |

> 📌 Make sure you are logged into your Home Assistant instance in the same browser before clicking the import buttons.

---

## 📁 Manual Installation

If you prefer manual installation:

1. Download the YAML files from the Gist links above  
2. In Home Assistant, go to:  
   **Settings → Automations & Scenes → Blueprints**  
3. Click **Import Blueprint**  
4. Upload the downloaded files

---

## ⚙️ Blueprint Configuration

### 1️⃣ Play Detection
- Monitors Apple TV or Chromecast media state  
- Turns ON Movie Mode when playback starts

### 2️⃣ Stop / Pause Detection
- Monitors media stop or pause events  
- Turns OFF Movie Mode

### 3️⃣ Lights & Covers Snapshot / Restore
- Saves the current state of selected lights and covers  
- Closes covers when Movie Mode starts  
- Restores lights and covers after Movie Mode ends with a configurable delay  
- Optional light fade-in transition  
- Prevents restore if Movie Mode is re-enabled during the delay

---

## 🧠 Recommended Setup

- Create an `input_boolean.movie_mode` to control Movie Mode  
- Use **Play Detection** to turn ON the input_boolean when media starts playing  
- Use **Stop / Pause Detection** to turn OFF the input_boolean when media pauses or stops  
- Use **Lights & Covers Snapshot / Restore** to automatically save and restore lighting and cover positions

---

## 💡 Contribution & Development

Ideas, improvements, or new blueprints are welcome!  

You can:
- Open an **Issue** for feature requests or bugs  
- Submit a **Pull Request**  
- Leave a ⭐ if you find this useful 🙂

---

## 📜 License

This project is licensed under the **MIT License**.  
You are free to use, modify, and share it.

---

**Author:** Nero  
**Platform:** Home Assistant
