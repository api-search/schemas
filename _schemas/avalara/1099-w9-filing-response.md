---
description: FilingResponse schema from Avalara API
layout: schema
name: FilingResponse
properties_list:
- description: ''
  name: filingId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: formCount
  type: integer
- description: ''
  name: submittedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/1099-w9-filing-response-schema.json
slug: 1099-w9-filing-response
source_filename: 1099-w9-filing-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-filing-response-schema.json\",\n  \"title\": \"FilingResponse\",\n  \"description\": \"FilingResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filingId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Accepted\",\n        \"Processing\",\n        \"Rejected\"\n      ]\n    },\n    \"formCount\": {\n      \"type\": \"integer\"\n    },\n    \"submittedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-filing-response-schema.json
tags:
- Taxes
title: FilingResponse
---
