# Appletv-blueprints
Home Assistant blueprints for Apple TV and Chromecast automations
# 📺 Home Assistant Blueprints – Apple TV & Movie Mode

A collection of blueprints for **Home Assistant** automation related to Apple TV, Chromecast, and “Movie Mode”.

## 🎬 Movie Mode – Save & Restore (Lights + Covers)

This blueprint allows you to:
- Save the current state of selected lights and covers,
- Close covers when Movie Mode is activated,
- Restore previous light and cover states after Movie Mode is deactivated with a configurable delay.

### 📥 Quick Import to Home Assistant

Click the button below to open the import screen directly in your Home Assistant instance:

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?url=https://raw.githubusercontent.com/nero-Ha/Appletv-blueprints/main/movie_mode_save_restore.yaml)

> 📌 Make sure you are logged into your Home Assistant instance in your browser.

---

## 📁 Manual Installation

1. Download the `movie_mode_save_restore.yaml` file from this repository.
2. In **Home Assistant UI**, go to:  
   **Settings → Automations & Scenes → Blueprints**
3. Click **Import Blueprint**
4. Choose the downloaded file and finish the import.

---

## ⚙️ Blueprint Configuration

The blueprint provides the following inputs:

| Input | Description |
|-------|-------------|
| *Movie Mode helper* | `input_boolean` to control the Movie Mode state |
| *Lights* | List of lights to snapshot and restore |
| *Covers* | List of covers (blinds/curtains) to close and restore positions |
| *Restore delay* | Delay time before restoring lights and covers |
| *Light transition* | Fade-in duration for lights when restoring |

---

## 💡 Contribution & Development

Have ideas for improvements or new blueprints?  
You can:
- Open an *issue* to suggest a feature,
- Submit a *pull request* with your code,
- Leave a ⭐ if you like the project 😊

---

## 📜 License

This project is licensed under the **MIT License** — use, modify, and share freely.
