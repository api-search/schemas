---
description: FlowValidationError from WhatsApp API
layout: schema
name: FlowValidationError
properties_list:
- description: ''
  name: error
  type: string
- description: ''
  name: error_type
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: line_start
  type: integer
- description: ''
  name: line_end
  type: integer
- description: ''
  name: column_start
  type: integer
- description: ''
  name: column_end
  type: integer
- description: ''
  name: pointers
  type: array
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-flows-api-flow-validation-error-schema.json
slug: whatsapp-flows-api-flow-validation-error
source_filename: whatsapp-flows-api-flow-validation-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-flow-validation-error-schema.json\",\n  \"title\": \"FlowValidationError\",\n  \"description\": \"FlowValidationError from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"error_type\": {\n      \"type\": \"string\",\n      \"example\": \"text\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Hello from WhatsApp!\"\n    },\n    \"line_start\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"line_end\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"column_start\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"column_end\": {\n      \"type\": \"integer\",\n      \"example\": 42\n  \
  \  },\n    \"pointers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-flow-validation-error-schema.json
tags: []
title: FlowValidationError
---
