---
description: Schema for a Rainbow CPaaS message object
layout: schema
name: Rainbow Message
properties_list:
- description: Unique message identifier
  name: id
  type: string
- description: Text content of the message
  name: content
  type: string
- description: Sender's contact ID
  name: from
  type: string
- description: Recipient contact ID or bubble ID
  name: to
  type: string
- description: Message type
  name: type
  type: string
- description: ISO 8601 creation timestamp
  name: timestamp
  type: string
- description: Message delivery status
  name: status
  type: string
provider_name: Rainbow
provider_slug: rainbow
schema_file: json-schema/rainbow-message-schema.json
slug: rainbow-message
source_filename: rainbow-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://openrainbow.com/schemas/message\",\n  \"title\": \"Rainbow Message\",\n  \"description\": \"Schema for a Rainbow CPaaS message object\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"content\", \"from\", \"to\", \"type\", \"timestamp\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique message identifier\"\n    },\n    \"content\": {\n      \"type\": \"string\",\n      \"description\": \"Text content of the message\"\n    },\n    \"from\": {\n      \"type\": \"string\",\n      \"description\": \"Sender's contact ID\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient contact ID or bubble ID\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\"chat\", \"groupchat\"],\n      \"description\": \"Message type\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\",\n     \
  \ \"format\": \"date-time\",\n      \"description\": \"ISO 8601 creation timestamp\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"sent\", \"delivered\", \"read\"],\n      \"description\": \"Message delivery status\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/rainbow/refs/heads/main/json-schema/rainbow-message-schema.json
tags:
- Communications
- CPaaS
- Chat
- Voice
- Video
- Telephony
- Messaging
- Collaboration
- Unified Communications
title: Rainbow Message
---
