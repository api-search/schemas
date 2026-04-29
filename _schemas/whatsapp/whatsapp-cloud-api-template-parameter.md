---
description: TemplateParameter from WhatsApp API
layout: schema
name: TemplateParameter
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: text
  type: string
- description: ''
  name: payload
  type: string
- description: ''
  name: coupon_code
  type: string
- description: ''
  name: image
  type: object
- description: ''
  name: video
  type: object
- description: ''
  name: document
  type: object
- description: ''
  name: location
  type: object
- description: ''
  name: currency
  type: object
- description: ''
  name: date_time
  type: object
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-cloud-api-template-parameter-schema.json
slug: whatsapp-cloud-api-template-parameter
source_filename: whatsapp-cloud-api-template-parameter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-template-parameter-schema.json\",\n  \"title\": \"TemplateParameter\",\n  \"description\": \"TemplateParameter from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"text\",\n        \"image\",\n        \"video\",\n        \"document\",\n        \"location\",\n        \"currency\",\n        \"date_time\",\n        \"payload\",\n        \"coupon_code\"\n      ],\n      \"example\": \"text\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"example\": \"Hello from WhatsApp!\"\n    },\n    \"payload\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"coupon_code\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"image\": {\n\
  \      \"$ref\": \"#/components/schemas/MediaObject\"\n    },\n    \"video\": {\n      \"$ref\": \"#/components/schemas/MediaObject\"\n    },\n    \"document\": {\n      \"$ref\": \"#/components/schemas/DocumentObject\"\n    },\n    \"location\": {\n      \"$ref\": \"#/components/schemas/LocationMessage\"\n    },\n    \"currency\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fallback_value\": {\n          \"type\": \"string\"\n        },\n        \"code\": {\n          \"type\": \"string\"\n        },\n        \"amount_1000\": {\n          \"type\": \"integer\"\n        }\n      }\n    },\n    \"date_time\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"fallback_value\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-cloud-api-template-parameter-schema.json
tags: []
title: TemplateParameter
---
