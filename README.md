[![Add to Home Assistant](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?repository_url=https://github.com/Bradw-17/frigate-ai-notifications/blob/main/frigate_ai_notification.yaml)

# Frigate AI Notifications (v2.0)

🚨 AI-enhanced camera notifications for Frigate using either **LLM Vision** or **AI Task**.  
📱 Sends rich media notifications to mobile devices using Home Assistant Companion App.

---

## 📌 Features

- Dual integration: LLM Vision or AI Task (Home Assistant 2025.8+)
- Snapshot + clip analysis with model selection
- Smart object + zone filtering
- Dynamic priority notifications
- Native mobile notifications with media
- Cooldown timer for per-camera alert throttling

---

## 🔧 Setup Instructions

1. Install either:
   - [AI Task](https://www.home-assistant.io/integrations/ai_task/) (HA 2025.8+)
   - [LLM Vision](https://github.com/valentinfrlch/ha-llmvision)

2. Configure Frigate with MQTT

3. Set up your External URL under **Settings > System > Network**

4. Import the blueprint using the button above, or manually:
   - Settings → Automations & Scenes → Blueprints → Import Blueprint
   - Paste:
     ```
     https://github.com/Bradw-17/frigate-ai-notifications/blob/main/frigate_ai_notification.yaml
     ```

5. Create a new automation using the blueprint and configure inputs

---

## 🧠 Supported Models

- OpenAI: `gpt-4o`, `gpt-4.1`, `gpt-4o-mini`
- Claude: `claude-3-5-haiku`, `claude-sonnet`, `claude-opus`
- Gemini: `gemini-1.5`, `gemini-2.0`, `gemini-2.5`
- Meta LLaMA: `llama-3`, `llama-4-scout`, `llama-4-maverick`
- Custom or local models via Ollama or LocalAI

---

## 💡 Example Use Cases

- Detect and summarize driveway visitors
- Notify when a face or license plate is captured
- Alert when cars pull up to the house
- Reduce false positives with object + zone matching

---

## 🛠️ GitHub

https://github.com/Bradw-17/frigate-ai-notifications

Issues or suggestions? Post in the [Home Assistant forums](https://community.home-assistant.io/c/blueprints-exchange/53) or open a GitHub issue.
