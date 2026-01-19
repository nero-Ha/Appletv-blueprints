# 📺 Appletv-blueprints

Home Assistant blueprints for **Apple TV**, **Chromecast**, and **Movie Mode** automations.

A small collection of clean, reusable blueprints focused on media-based lighting and cover control.

---

## 🎬 Quick Import of Blueprints

You can import the following blueprints directly into your Home Assistant instance by clicking the links below or using the URLs in HA → Import Blueprint.

| Blueprint | Description | Import Link |
|-----------|-------------|------------|
| **Movie Mode ON / Play Detection** | Detects when Apple TV or Chromecast starts playing media and turns ON Movie Mode | [Import](https://gist.githubusercontent.com/nero-Ha/7d25335bf65c94c4c428ace105856a81/raw/3b933c1a51aa940eafd6e8ac1369a7ebb5a68c39/appletvplayNero.yaml) |
| **Movie Mode OFF / Pause Detection** | Detects when media is paused or stopped and turns OFF Movie Mode | [Import](https://gist.githubusercontent.com/nero-Ha/89c419fad7593fd07a82958e88249e3d/raw/a97c5f22d90e009d8edc2d374d38d08c89510fd1/appletvpauseNero.yaml) |
| **Lights & Covers Snapshot / Restore** | Saves the current state of lights and covers, closes covers when Movie Mode starts, and restores them after Movie Mode ends | [Import](https://gist.githubusercontent.com/nero-Ha/e6379e81975b4606fa520f24b82e46b2/raw/3f5fdb3644bb12a7783b0ae7a0568a4da25ed8b7/movie_mode_save_restore.yaml) |

> 📌 Make sure you are logged into your Home Assistant instance in the same browser before importing.

---

## 📁 Manual Installation

If you prefer manual installation:

1. Download the YAML files from the links above.  
2. In Home Assistant, go to:  
   **Settings → Automations & Scenes → Blueprints**  
3. Click **Import Blueprint**  
4. Paste the RAW URL or upload the downloaded YAML files.

---

## ⚙️ Blueprint Configuration

### 1️⃣ Movie Mode ON / Play Detection
- Monitors Apple TV or Chromecast media state.  
- Turns ON the `input_boolean.movie_mode` when media starts playing.

### 2️⃣ Movie Mode OFF / Pause Detection
- Monitors media pause or stop events.  
- Turns OFF the `input_boolean.movie_mode`.

### 3️⃣ Lights & Covers Snapshot / Restore
- Saves the current state of selected lights and covers.  
- Closes covers when Movie Mode starts.  
- Restores lights and covers after Movie Mode ends with a configurable delay.  
- Optional light fade-in transition.  
- Prevents restore if Movie Mode is re-enabled during the delay.

---

## 🧠 Recommended Setup

- Create an `input_boolean.movie_mode` to control Movie Mode.  
- Use **Movie Mode ON / Play Detection** to turn ON the input_boolean when media starts.  
- Use **Movie Mode OFF / Pause Detection** to turn OFF the input_boolean when media pauses or stops.  
- Use **Lights & Covers Snapshot / Restore** to automatically save and restore lighting and cover positions.

---

## 💡 Contribution & Development

Ideas, improvements, or new blueprints are welcome!  

You can:  
- Open an **Issue** for feature requests or bugs.  
- Submit a **Pull Request**.  
- Leave a ⭐ if you find this useful 🙂

---

## 📜 License

This project is licensed under the **MIT License**.  
You are free to use, modify, and share it.

---

**Author:** Nero  
**Platform:** Home Assistant
