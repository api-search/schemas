---
description: ''
layout: schema
name: SubscriptionRequest
properties_list:
- description: The type of change to subscribe to.
  name: changeType
  type: string
- description: The URL to receive change notifications.
  name: notificationUrl
  type: string
- description: The resource path to subscribe to. For Copilot interactions use /copilot/interactionHistory/getAllEnterpriseInteractions.
  name: resource
  type: string
- description: The date and time when the subscription expires.
  name: expirationDateTime
  type: string
- description: Optional client state value included in each notification for validation.
  name: clientState
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-subscription-request-schema.json
slug: microsoft-copilot-subscription-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SubscriptionRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"changeType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of change to subscribe to.\"\n    },\n    \"notificationUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL to receive change notifications.\"\n    },\n    \"resource\": {\n      \"type\": \"string\",\n      \"description\": \"The resource path to subscribe to. For Copilot interactions use /copilot/interactionHistory/getAllEnterpriseInteractions.\"\n    },\n    \"expirationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time when the subscription expires.\"\n    },\n    \"clientState\": {\n      \"type\": \"string\",\n      \"description\": \"Optional client state value included in each notification for validation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-subscription-request-schema.json
tags:
- Agents
- AI Assistant
- Artificial Intelligence
- Chatbot
- Copilot
- Extensibility
- Generative AI
- Microsoft 365
- Productivity
title: SubscriptionRequest
---
