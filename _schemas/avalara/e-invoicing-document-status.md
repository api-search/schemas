---
description: DocumentStatus schema from Avalara API
layout: schema
name: DocumentStatus
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: statusDate
  type: string
- description: ''
  name: events
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/e-invoicing-document-status-schema.json
slug: e-invoicing-document-status
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-status-schema.json\",\n  \"title\": \"DocumentStatus\",\n  \"description\": \"DocumentStatus schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Pending\",\n        \"Accepted\",\n        \"Rejected\",\n        \"Error\"\n      ]\n    },\n    \"statusDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"events\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DocumentEvent\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/e-invoicing-document-status-schema.json
tags:
- Taxes
title: DocumentStatus
---
