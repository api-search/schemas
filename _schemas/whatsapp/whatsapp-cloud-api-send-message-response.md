---
description: SendMessageResponse from WhatsApp API
layout: schema
name: SendMessageResponse
properties_list:
- description: ''
  name: messaging_product
  type: string
- description: ''
  name: contacts
  type: array
- description: ''
  name: messages
  type: array
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-send-message-response-schema.json
slug: whatsapp-cloud-api-send-message-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-send-message-response-schema.json\",\n  \"title\": \"SendMessageResponse\",\n  \"description\": \"SendMessageResponse from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messaging_product\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"input\": {\n            \"type\": \"string\"\n          },\n          \"wa_id\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"messages\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\":\
  \ \"WhatsApp message ID\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-send-message-response-schema.json
tags: []
title: SendMessageResponse
---
