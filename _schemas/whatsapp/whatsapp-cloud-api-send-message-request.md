---
description: SendMessageRequest from WhatsApp API
layout: schema
name: SendMessageRequest
properties_list:
- description: ''
  name: messaging_product
  type: string
- description: ''
  name: recipient_type
  type: string
- description: Recipient phone number in E.164 format without the leading +
  name: to
  type: string
- description: ''
  name: type
  type: string
- description: Context for reply messages
  name: context
  type: object
- description: Arbitrary string for tracking, returned in webhooks
  name: biz_opaque_callback_data
  type: string
- description: Set to read to mark an incoming message as read
  name: status
  type: string
- description: ID of the message to mark as read (required when status is read)
  name: message_id
  type: string
- description: ''
  name: text
  type: object
- description: ''
  name: image
  type: object
- description: ''
  name: video
  type: object
- description: ''
  name: audio
  type: object
- description: ''
  name: document
  type: object
- description: ''
  name: sticker
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: contacts
  type: array
- description: ''
  name: interactive
  type: object
- description: ''
  name: template
  type: object
- description: ''
  name: reaction
  type: object
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-send-message-request-schema.json
slug: whatsapp-cloud-api-send-message-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-send-message-request-schema.json\",\n  \"title\": \"SendMessageRequest\",\n  \"description\": \"SendMessageRequest from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"messaging_product\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"whatsapp\"\n      ],\n      \"example\": \"whatsapp\"\n    },\n    \"recipient_type\": {\n      \"type\": \"string\",\n      \"default\": \"individual\",\n      \"example\": \"text\"\n    },\n    \"to\": {\n      \"type\": \"string\",\n      \"description\": \"Recipient phone number in E.164 format without the leading +\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"text\",\n        \"image\",\n        \"video\",\n        \"audio\",\n        \"document\"\
  ,\n        \"sticker\",\n        \"location\",\n        \"contacts\",\n        \"interactive\",\n        \"template\",\n        \"reaction\"\n      ],\n      \"example\": \"text\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Context for reply messages\",\n      \"properties\": {\n        \"message_id\": {\n          \"type\": \"string\",\n          \"description\": \"ID of the message being replied to\"\n        }\n      }\n    },\n    \"biz_opaque_callback_data\": {\n      \"type\": \"string\",\n      \"description\": \"Arbitrary string for tracking, returned in webhooks\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"read\"\n      ],\n      \"description\": \"Set to read to mark an incoming message as read\",\n      \"example\": \"read\"\n    },\n    \"message_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the message to mark as read (required when\
  \ status is read)\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"text\": {\n      \"$ref\": \"#/components/schemas/TextMessage\"\n    },\n    \"image\": {\n      \"$ref\": \"#/components/schemas/MediaObject\"\n    },\n    \"video\": {\n      \"$ref\": \"#/components/schemas/MediaObject\"\n    },\n    \"audio\": {\n      \"$ref\": \"#/components/schemas/AudioObject\"\n    },\n    \"document\": {\n      \"$ref\": \"#/components/schemas/DocumentObject\"\n    },\n    \"sticker\": {\n      \"$ref\": \"#/components/schemas/StickerObject\"\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/LocationMessage\"\n    },\n    \"contacts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ContactObject\"\n      }\n    },\n    \"interactive\": {\n      \"$ref\": \"#/components/schemas/InteractiveMessage\"\n    },\n    \"template\": {\n      \"$ref\": \"#/components/schemas/TemplateMessage\"\n    },\n    \"reaction\": {\n      \"$ref\"\
  : \"#/components/schemas/ReactionMessage\"\n    }\n  },\n  \"required\": [\n    \"messaging_product\",\n    \"to\",\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-send-message-request-schema.json
tags: []
title: SendMessageRequest
---
