---
description: TemplateComponent from WhatsApp API
layout: schema
name: TemplateComponent
properties_list:
- description: ''
  name: type
  type: string
- description: Required for button components
  name: sub_type
  type: string
- description: Button index (required for button components)
  name: index
  type: string
- description: ''
  name: parameters
  type: array
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-template-component-schema.json
slug: whatsapp-cloud-api-template-component
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-template-component-schema.json\",\n  \"title\": \"TemplateComponent\",\n  \"description\": \"TemplateComponent from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"header\",\n        \"body\",\n        \"button\"\n      ],\n      \"example\": \"header\"\n    },\n    \"sub_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"quick_reply\",\n        \"url\",\n        \"copy_code\",\n        \"flow\",\n        \"catalog\"\n      ],\n      \"description\": \"Required for button components\",\n      \"example\": \"quick_reply\"\n    },\n    \"index\": {\n      \"type\": \"string\",\n      \"description\": \"Button index (required for button components)\",\n      \"example\": \"example_value\"\
  \n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TemplateParameter\"\n      }\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-template-component-schema.json
tags: []
title: TemplateComponent
---
