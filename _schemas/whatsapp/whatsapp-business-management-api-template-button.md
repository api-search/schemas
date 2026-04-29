---
description: TemplateButton from WhatsApp API
layout: schema
name: TemplateButton
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: text
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: phone_number
  type: string
- description: ''
  name: example
  type: string
- description: ''
  name: flow_id
  type: string
- description: ''
  name: flow_action
  type: string
- description: ''
  name: navigate_screen
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-business-management-api-template-button-schema.json
slug: whatsapp-business-management-api-template-button
source_filename: whatsapp-business-management-api-template-button-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-template-button-schema.json\",\n  \"title\": \"TemplateButton\",\n  \"description\": \"TemplateButton from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"QUICK_REPLY\",\n        \"URL\",\n        \"PHONE_NUMBER\",\n        \"COPY_CODE\",\n        \"FLOW\",\n        \"OTP\",\n        \"CATALOG\",\n        \"MPM\"\n      ],\n      \"example\": \"QUICK_REPLY\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"example\": \"Hello from WhatsApp!\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://example.com/image.jpg\"\n    },\n    \"phone_number\": {\n      \"type\": \"string\",\n      \"example\": \"+15551234567\"\n \
  \   },\n    \"example\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"flow_id\": {\n      \"type\": \"string\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"flow_action\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"navigate_screen\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"text\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-template-button-schema.json
tags: []
title: TemplateButton
---
