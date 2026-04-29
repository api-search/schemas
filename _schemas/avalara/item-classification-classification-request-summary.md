---
description: ClassificationRequestSummary schema from Avalara API
layout: schema
name: ClassificationRequestSummary
properties_list:
- description: ''
  name: requestId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: itemCount
  type: integer
- description: ''
  name: submittedDate
  type: string
- description: ''
  name: completedDate
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/item-classification-classification-request-summary-schema.json
slug: item-classification-classification-request-summary
source_filename: item-classification-classification-request-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-request-summary-schema.json\",\n  \"title\": \"ClassificationRequestSummary\",\n  \"description\": \"ClassificationRequestSummary schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"requestId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"itemCount\": {\n      \"type\": \"integer\"\n    },\n    \"submittedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"completedDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/item-classification-classification-request-summary-schema.json
tags:
- Taxes
title: ClassificationRequestSummary
---
