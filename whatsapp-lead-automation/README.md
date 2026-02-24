# WhatsApp Lead Automation Demo

## Overview

This system simulates a WhatsApp automation backend using n8n.

It demonstrates how businesses can:

- Receives a webhook request (simulating WhatsApp incoming message)
- Reads predefined rules from Google Sheets
- Matches keywords dynamically
- Logs the interaction
- Returns an automated response

## Architecture

Webhook → Google Sheets (rules) → Code logic → Google Sheets (lead capture) → JSON Response

## Example Request

```json
{
  "from": "+541112345678",
  "message": "precio"
}
```

## Example Response

```json
{
  "from": "+541112345678",
  "message": "precio",
  "response": "Nuestro precio es $100"
}
```

## Use Case

Ideal for:
- Small businesses
- Clinics
- Real estate agencies
-E-commerce stores
-Service providers receiving high WhatsApp volume

Tech Stack:
- n8n (self-hosted)
- Google Sheets API
- Docker
- JavaScript (custom logic node)

Author:
- Built by Francisco Premuz

