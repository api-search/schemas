---
description: TemplateMessage from WhatsApp API
layout: schema
name: TemplateMessage
properties_list:
- description: Template name
  name: name
  type: string
- description: ''
  name: language
  type: object
- description: ''
  name: components
  type: array
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-template-message-schema.json
slug: whatsapp-cloud-api-template-message
source_filename: whatsapp-cloud-api-template-message-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-template-message-schema.json\",\n  \"title\": \"TemplateMessage\",\n  \"description\": \"TemplateMessage from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Template name\",\n      \"example\": \"Example Business\"\n    },\n    \"language\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"code\"\n      ],\n      \"properties\": {\n        \"code\": {\n          \"type\": \"string\",\n          \"description\": \"Language/locale code\"\n        },\n        \"policy\": {\n          \"type\": \"string\",\n          \"default\": \"deterministic\"\n        }\n      }\n    },\n    \"components\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TemplateComponent\"\
  \n      }\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"language\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-template-message-schema.json
tags: []
title: TemplateMessage
---
