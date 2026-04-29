---
description: TextMessage from WhatsApp API
layout: schema
name: TextMessage
properties_list:
- description: Message text
  name: body
  type: string
- description: Set true to render URL previews
  name: preview_url
  type: boolean
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-text-message-schema.json
slug: whatsapp-cloud-api-text-message
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-text-message-schema.json\",\n  \"title\": \"TextMessage\",\n  \"description\": \"TextMessage from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"body\": {\n      \"type\": \"string\",\n      \"description\": \"Message text\",\n      \"maxLength\": 4096,\n      \"example\": \"Hello from WhatsApp!\"\n    },\n    \"preview_url\": {\n      \"type\": \"boolean\",\n      \"description\": \"Set true to render URL previews\",\n      \"default\": false,\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"body\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-text-message-schema.json
tags: []
title: TextMessage
---
