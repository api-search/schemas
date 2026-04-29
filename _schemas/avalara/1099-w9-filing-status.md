---
description: FilingStatus schema from Avalara API
layout: schema
name: FilingStatus
properties_list:
- description: ''
  name: filingId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: acceptedCount
  type: integer
- description: ''
  name: rejectedCount
  type: integer
- description: ''
  name: errors
  type: array
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/1099-w9-filing-status-schema.json
slug: 1099-w9-filing-status
source_filename: 1099-w9-filing-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-filing-status-schema.json\",\n  \"title\": \"FilingStatus\",\n  \"description\": \"FilingStatus schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"filingId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Processing\",\n        \"Accepted\",\n        \"AcceptedWithErrors\",\n        \"Rejected\"\n      ]\n    },\n    \"acceptedCount\": {\n      \"type\": \"integer\"\n    },\n    \"rejectedCount\": {\n      \"type\": \"integer\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"formId\": {\n            \"type\": \"string\"\n          },\n          \"errorCode\": {\n            \"type\": \"string\"\n          },\n\
  \          \"message\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/1099-w9-filing-status-schema.json
tags:
- Taxes
title: FilingStatus
---
