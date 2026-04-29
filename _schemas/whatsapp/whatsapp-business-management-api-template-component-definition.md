---
description: TemplateComponentDefinition from WhatsApp API
layout: schema
name: TemplateComponentDefinition
properties_list:
- description: ''
  name: type
  type: string
- description: Header format type
  name: format
  type: string
- description: Component text content
  name: text
  type: string
- description: Example values for variables
  name: example
  type: object
- description: ''
  name: buttons
  type: array
- description: Authentication templates only
  name: add_security_recommendation
  type: boolean
- description: Authentication templates only (1-90)
  name: code_expiration_minutes
  type: integer
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-business-management-api-template-component-definition-schema.json
slug: whatsapp-business-management-api-template-component-definition
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-template-component-definition-schema.json\",\n  \"title\": \"TemplateComponentDefinition\",\n  \"description\": \"TemplateComponentDefinition from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"HEADER\",\n        \"BODY\",\n        \"FOOTER\",\n        \"BUTTONS\"\n      ],\n      \"example\": \"HEADER\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"TEXT\",\n        \"IMAGE\",\n        \"VIDEO\",\n        \"DOCUMENT\",\n        \"LOCATION\"\n      ],\n      \"description\": \"Header format type\",\n      \"example\": \"TEXT\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Component text content\",\n      \"example\"\
  : \"Hello from WhatsApp!\"\n    },\n    \"example\": {\n      \"type\": \"object\",\n      \"description\": \"Example values for variables\"\n    },\n    \"buttons\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/TemplateButton\"\n      }\n    },\n    \"add_security_recommendation\": {\n      \"type\": \"boolean\",\n      \"description\": \"Authentication templates only\",\n      \"example\": true\n    },\n    \"code_expiration_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Authentication templates only (1-90)\",\n      \"minimum\": 1,\n      \"maximum\": 90,\n      \"example\": 42\n    }\n  },\n  \"required\": [\n    \"type\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-business-management-api-template-component-definition-schema.json
tags: []
title: TemplateComponentDefinition
---
