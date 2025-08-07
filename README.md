# 📸 Frigate AI Camera Notifications (v2.0)

This is a Home Assistant automation blueprint that enhances Frigate events using AI-generated summaries of snapshots and clips. Works with both the native **AI Task** integration (2025.8+) and **LLM Vision**.

---

## ✨ Features

- 🔍 AI analysis of **snapshots** and **video clips**
- 🧠 Supports both `ai_task` and `llmvision`
- 📱 Sends **rich push notifications** (image, video, summary)
- 🧠 Configurable prompts, token limits, model, provider
- 📊 Smart detection filtering (objects + zones)
- 🔁 Cooldown logic to avoid notification spam
- 🔔 Notification priority based on object types
- 📎 Optional context from entities

---

## ✅ Requirements

- [Frigate](https://docs.frigate.video/) + MQTT
- [Home Assistant 2025.8+](https://www.home-assistant.io/) (for `ai_task`) **OR**
  [LLM Vision](https://github.com/valentinfrlch/ha-llmvision)
- Mobile App integration with `notify.mobile_app_*`
- External URL set under `Settings > System > Network`

---

## 🚀 Installation

1. Copy the contents of [`frigate_ai_notification.yaml`](./frigate_ai_notification.yaml) into a new blueprint in Home Assistant **or** use the one-click button below:

[![Add to Home Assistant](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?repository_url=https://github.com/Bradw-17/frigate-ai-notifications&filename=frigate_ai_notification.yaml)

2. Fill in the required inputs:
   - Frigate camera
   - Device(s) to notify
   - Choose `ai_task` or `llmvision`
   - Set object labels (e.g. `person`, `car`)

---

## 🛠️ Configuration Inputs

The blueprint exposes a wide set of inputs:

- AI integration type and provider/model
- Detection object types (labels)
- Optional zone filtering
- Notification recipients
- Snapshot and clip prompts
- Temperature, token limit, and resolution
- High-priority labels (to adjust urgency)
- Entity context (for LLM Vision only)

---

## 💬 Community

You can find more info or contribute to the discussion on the [Home Assistant Community Forum post](https://community.home-assistant.io/t/ai-enhanced-frigate-camera-notifications-with-llm-support/).

---

## 📜 License

[MIT License](./LICENSE)

