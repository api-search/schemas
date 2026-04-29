---
description: CreateFlowRequest from WhatsApp API
layout: schema
name: CreateFlowRequest
properties_list:
- description: Flow display name
  name: name
  type: string
- description: ''
  name: categories
  type: array
- description: ID of existing flow to clone
  name: clone_flow_id
  type: string
- description: HTTPS endpoint for data exchange
  name: endpoint_uri
  type: string
provider_name: WhatsApp
provider_slug: whatsapp
schema_file: json-schema/whatsapp-flows-api-create-flow-request-schema.json
slug: whatsapp-flows-api-create-flow-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-create-flow-request-schema.json\",\n  \"title\": \"CreateFlowRequest\",\n  \"description\": \"CreateFlowRequest from WhatsApp API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Flow display name\",\n      \"example\": \"Example Business\"\n    },\n    \"categories\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"SIGN_UP\",\n          \"SIGN_IN\",\n          \"APPOINTMENT_BOOKING\",\n          \"LEAD_GENERATION\",\n          \"CONTACT_US\",\n          \"CUSTOMER_SUPPORT\",\n          \"SURVEY\",\n          \"OTHER\"\n        ]\n      }\n    },\n    \"clone_flow_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of existing flow to clone\"\
  ,\n      \"example\": \"wamid.abc123\"\n    },\n    \"endpoint_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"HTTPS endpoint for data exchange\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"name\",\n    \"categories\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/whatsapp/refs/heads/main/json-schema/whatsapp-flows-api-create-flow-request-schema.json
tags: []
title: CreateFlowRequest
---
