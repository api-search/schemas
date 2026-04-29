---
description: ProfitCenter schema from Aramark Marko API
layout: schema
name: ProfitCenter
properties_list:
- description: Profit center identifier
  name: id
  type: string
- description: Profit center name
  name: name
  type: string
- description: Profit center code
  name: code
  type: string
- description: Parent profit center identifier
  name: parentId
  type: string
- description: Whether the profit center is active
  name: active
  type: boolean
provider_name: Aramark
provider_slug: aramark
schema_file: json-schema/marko-api-profit-center-schema.json
slug: marko-api-profit-center
source_filename: marko-api-profit-center-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Profit center identifier\",\n      \"example\": \"PC-001\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Profit center name\",\n      \"example\": \"Campus Center Dining\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Profit center code\",\n      \"example\": \"NE-CC-001\"\n    },\n    \"parentId\": {\n      \"type\": \"string\",\n      \"description\": \"Parent profit center identifier\",\n      \"example\": \"PC-REGION-NE\"\n    },\n    \"active\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the profit center is active\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-profit-center-schema.json\",\n  \"title\"\
  : \"ProfitCenter\",\n  \"description\": \"ProfitCenter schema from Aramark Marko API\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/aramark/refs/heads/main/json-schema/marko-api-profit-center-schema.json
tags:
- Food Services
- Facilities Management
- Uniform Services
- Data Platform
- Fortune 500
title: ProfitCenter
---
