---
description: ReactionMessage from WhatsApp API
layout: schema
name: ReactionMessage
properties_list:
- description: ID of the message to react to
  name: message_id
  type: string
- description: Emoji character or empty string to remove reaction
  name: emoji
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-reaction-message-schema.json
slug: whatsapp-cloud-api-reaction-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-reaction-message-schema.json\",\n  \"title\": \"ReactionMessage\",\n  \"description\": \"ReactionMessage from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the message to react to\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"emoji\": {\n      \"type\": \"string\",\n      \"description\": \"Emoji character or empty string to remove reaction\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"message_id\",\n    \"emoji\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-reaction-message-schema.json
tags: []
title: ReactionMessage
---
