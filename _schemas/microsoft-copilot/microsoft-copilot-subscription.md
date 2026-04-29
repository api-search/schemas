---
description: ''
layout: schema
name: Subscription
properties_list:
- description: The unique identifier of the subscription.
  name: id
  type: string
- description: The resource being monitored.
  name: resource
  type: string
- description: The type of change being monitored.
  name: changeType
  type: string
- description: The URL receiving notifications.
  name: notificationUrl
  type: string
- description: When the subscription expires.
  name: expirationDateTime
  type: string
- description: The client state value for validation.
  name: clientState
  type: string
provider_name: Microsoft Copilot
provider_slug: microsoft-copilot
schema_file: json-schema/microsoft-copilot-subscription-schema.json
slug: microsoft-copilot-subscription
source_filename: microsoft-copilot-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the subscription.\"\n    },\n    \"resource\": {\n      \"type\": \"string\",\n      \"description\": \"The resource being monitored.\"\n    },\n    \"changeType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of change being monitored.\"\n    },\n    \"notificationUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The URL receiving notifications.\"\n    },\n    \"expirationDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"When the subscription expires.\"\n    },\n    \"clientState\": {\n      \"type\": \"string\",\n      \"description\": \"The client state value for validation.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-copilot/refs/heads/main/json-schema/microsoft-copilot-subscription-schema.json
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
title: Subscription
---
