# 📺 Appletv-blueprints

Home Assistant blueprints for **Apple TV**, **Chromecast**, and **Movie Mode** automations.

A small collection of clean, reusable blueprints focused on media-based lighting and cover control.

---

## 🎬 Movie Mode – Save & Restore (Lights + Covers)

This blueprint allows you to automatically manage lights and covers when watching movies.

### ✨ Features
- 📸 Saves the current state of selected **lights**
- 🪟 Saves and restores **cover positions**
- 🎥 Closes covers when Movie Mode starts
- ⏱️ Restores lights and covers after Movie Mode ends with a configurable delay
- 🎚️ Optional light fade-in transition
- 🛑 Prevents restore if Movie Mode is re-enabled during the delay

Perfect for cinema or TV setups where pausing playback briefly should not immediately change lighting.

---

## 📥 Quick Import to Home Assistant

Click the button below to import the blueprint directly into your Home Assistant instance:

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](
https://my.home-assistant.io/redirect/blueprint_import/?url=https://gist.githubusercontent.com/nero-Ha/e6379e81975b4606fa520f24b82e46b2/raw/movie_mode_save_restore.yaml
)

> 📌 Make sure you are logged into your Home Assistant instance in the same browser.

---

## 📁 Manual Installation

If you prefer manual installation:

1. Download `movie_mode_save_restore.yaml` from the Gist link above  
2. In Home Assistant go to:  
   **Settings → Automations & Scenes → Blueprints**
3. Click **Import Blueprint**
4. Upload the downloaded file

---

## ⚙️ Blueprint Configuration

The blueprint provides the following inputs:

| Input | Description |
|------|-------------|
| **Movie Mode helper** | `input_boolean` controlling Movie Mode (ON = playing, OFF = paused/stopped) |
| **Lights** | Lights to snapshot and restore |
| **Covers** | Covers (blinds / curtains) to close and restore |
| **Restore delay** | Time to wait before restoring lights and covers |
| **Light transition** | Fade-in duration when restoring lights |

---

## 🧠 Recommended Setup

- Create one `input_boolean` named for example:  
  `input_boolean.movie_mode`
- Use this blueprint together with:
  - Apple TV `media_player.state`
  - Chromecast `media_player.state`
- Trigger Movie Mode ON when media starts playing  
- Trigger Movie Mode OFF when media is paused or stopped

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
