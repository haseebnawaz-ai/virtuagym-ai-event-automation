# 🏋️‍♂️ Virtuagym Event Automation Engine (AI Multi-Branch Router)

An enterprise-grade, event-driven AI automation system built with **n8n** and **Groq Chat Models (Llama-3)**. This system catches real-time webhooks from gym/fitness CRMs (Virtuagym), dynamically routes incoming event payloads, and generates personalized AI communication sequences in real time.

---

## 📐 System Architecture

![Workflow Architecture](./architecture.png)

---

## ⚡ Core Features & Logic

- **Real-Time Webhook Listener:** Instantly catches incoming gym member events and lifecycle triggers.
- **Dynamic Event Routing:** Evaluates payload conditions and branches into 6 dedicated execution paths:
  1. **New Lead Outreach:** Instant personalized engagement for incoming prospects.
  2. **Trial Conversion Offer:** AI-generated conversion offers for expiring trial accounts.
  3. **Member Check-in Follow-up:** Re-engagement messages based on attendance metrics.
  4. **Birthday Greeting:** Automated personalized birthday offers.
  5. **Onboarding Welcome:** Guided setup sequences for new members.
  6. **Renewal Reminder:** Timely expiration notices and renewal pushes.
- **High-Speed AI Generation:** Powered by **Groq Chat Models** for low-latency, hyper-contextual message crafting.
- **Automated Delivery:** Seamless integration with Gmail API for multi-channel message dispatch.

---

## 🛠️ Tech Stack

- **Orchestration:** n8n
- **AI Models:** Groq (Llama-3) / OpenAI API
- **Triggers & Data Handling:** Webhooks, Custom Code (JavaScript)
- **Integrations:** Virtuagym CRM, Gmail API

---

## 🚀 How to Import

1. Download the `workflow.json` file from this repository.
2. Open your **n8n** instance.
3. Click **Workflows ➔ Import from File** and select `workflow.json`.
4. Configure your **Groq API Key** and **Gmail OAuth2 credentials** in the respective nodes.
5. Activate the workflow and link your webhook endpoint to your CRM.
