---
description: Flow from WhatsApp API
layout: schema
name: Flow
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
  name: categories
  type: array
- description: ''
  name: validation_errors
  type: array
- description: ''
  name: json_version
  type: string
- description: ''
  name: data_api_version
  type: string
- description: ''
  name: endpoint_uri
  type: string
- description: ''
  name: preview
  type: object
- description: ''
  name: whatsapp_business_account
  type: object
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-flows-api-flow-schema.json
slug: whatsapp-flows-api-flow
source_filename: whatsapp-flows-api-flow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-flow-schema.json\",\n  \"title\": \"Flow\",\n  \"description\": \"Flow from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"wamid.abc123\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Business\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"DRAFT\",\n        \"PUBLISHED\",\n        \"DEPRECATED\",\n        \"BLOCKED\",\n        \"THROTTLED\"\n      ],\n      \"example\": \"DRAFT\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"SIGN_UP\",\n          \"SIGN_IN\",\n          \"APPOINTMENT_BOOKING\",\n          \"LEAD_GENERATION\",\n         \
  \ \"CONTACT_US\",\n          \"CUSTOMER_SUPPORT\",\n          \"SURVEY\",\n          \"OTHER\"\n        ]\n      }\n    },\n    \"validation_errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/FlowValidationError\"\n      }\n    },\n    \"json_version\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"data_api_version\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"endpoint_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"example_value\"\n    },\n    \"preview\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"preview_url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        },\n        \"expires_at\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"id\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"whatsapp_business_account\"\
  : {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-flow-schema.json
tags: []
title: Flow
---
