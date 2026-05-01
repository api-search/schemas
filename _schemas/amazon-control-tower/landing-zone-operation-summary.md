---
description: Summary of a landing zone operation.
layout: schema
name: LandingZoneOperationSummary
properties_list:
- description: The unique identifier of the operation.
  name: operationIdentifier
  type: string
- description: The type of the operation.
  name: operationType
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: status
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/landing-zone-operation-summary-schema.json
slug: landing-zone-operation-summary
source_filename: landing-zone-operation-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/landing-zone-operation-summary-schema.json\",\n  \"title\": \"LandingZoneOperationSummary\",\n  \"description\": \"Summary of a landing zone operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"operationIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the operation.\"\n    },\n    \"operationType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the operation.\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"IN_PROGRESS\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/landing-zone-operation-summary-schema.json
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: LandingZoneOperationSummary
---
