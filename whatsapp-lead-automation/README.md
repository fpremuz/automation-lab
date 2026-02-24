# 🤖 WhatsApp Keyword Automation Demo
## Overview

This project demonstrates a WhatsApp-style automation system built with n8n.

The workflow:

- Receives a webhook request (simulating WhatsApp incoming message)
- Reads predefined rules from Google Sheets
- Matches keywords dynamically
- Logs the interaction
- Returns an automated response

## 🔄 Workflow Architecture

Webhook
→ Google Sheets (Read Rules)
→ Code (Match Keywords)
→ Google Sheets (Log Interaction)
→ Respond to Webhook

## 🧠 Features

- Dynamic keyword matching
- Rule management via Google Sheets (no code changes required)
- Logging system
- Production-ready webhook response
- Docker-based local deployment

## 🚀 How to Run Locally

Install Docker

Run:

```
docker compose up -d
```

Open:

```
http://localhost:5678
```

Import the workflow JSON

🧪 Test Request Example
```
curl -X POST http://localhost:5678/webhook/whatsapp-demo \
-H "Content-Type: application/json" \
-d '{"from":"+123456789","message":"precio"}'
```

## 💼 Use Cases

- WhatsApp customer support automation
- Lead qualification
- FAQ automation
- Appointment booking pre-filter
