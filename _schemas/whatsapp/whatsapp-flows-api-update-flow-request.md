---
description: UpdateFlowRequest from WhatsApp API
layout: schema
name: UpdateFlowRequest
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: categories
  type: array
- description: ''
  name: endpoint_uri
  type: string
- description: ''
  name: application_id
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-flows-api-update-flow-request-schema.json
slug: whatsapp-flows-api-update-flow-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-update-flow-request-schema.json\",\n  \"title\": \"UpdateFlowRequest\",\n  \"description\": \"UpdateFlowRequest from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Business\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"endpoint_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"example_value\"\n    },\n    \"application_id\": {\n      \"type\": \"string\",\n      \"example\": \"wamid.abc123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-update-flow-request-schema.json
tags: []
title: UpdateFlowRequest
---
