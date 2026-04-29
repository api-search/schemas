---
description: MessageTemplate from WhatsApp API
layout: schema
name: MessageTemplate
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: language
  type: string
- description: ''
  name: components
  type: array
- description: ''
  name: parameter_format
  type: string
- description: ''
  name: quality_score
  type: object
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-business-management-api-message-template-schema.json
slug: whatsapp-business-management-api-message-template
source_filename: whatsapp-business-management-api-message-template-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-message-template-schema.json\",\n  \"title\": \"MessageTemplate\",\n  \"description\": \"MessageTemplate from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Business\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"APPROVED\",\n        \"PENDING\",\n        \"REJECTED\",\n        \"PAUSED\",\n        \"DISABLED\"\n      ],\n      \"example\": \"APPROVED\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"AUTHENTICATION\",\n        \"MARKETING\",\n        \"UTILITY\"\n      ],\n      \"example\": \"AUTHENTICATION\"\n    },\n\
  \    \"language\": {\n      \"type\": \"string\",\n      \"example\": \"en_US\"\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TemplateComponentDefinition\"\n      }\n    },\n    \"parameter_format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POSITIONAL\",\n        \"NAMED\"\n      ],\n      \"example\": \"POSITIONAL\"\n    },\n    \"quality_score\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"score\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-message-template-schema.json
tags: []
title: MessageTemplate
---
