---
description: Information about a landing zone operation.
layout: schema
name: LandingZoneOperationDetail
properties_list:
- description: The time the operation completed.
  name: endTime
  type: string
- description: The unique identifier of the operation.
  name: operationIdentifier
  type: string
- description: The type of landing zone operation.
  name: operationType
  type: string
- description: The time the operation was initiated.
  name: startTime
  type: string
- description: The status of the operation.
  name: status
  type: string
- description: If the operation result is FAILED, this string contains a message explaining why.
  name: statusMessage
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/landing-zone-operation-detail-schema.json
slug: landing-zone-operation-detail
source_filename: landing-zone-operation-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/landing-zone-operation-detail-schema.json\",\n  \"title\": \"LandingZoneOperationDetail\",\n  \"description\": \"Information about a landing zone operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the operation completed.\"\n    },\n    \"operationIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the operation.\"\n    },\n    \"operationType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of landing zone operation.\",\n      \"enum\": [\n        \"CREATE\",\n        \"UPDATE\",\n        \"RESET\",\n        \"DELETE\"\n      ]\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"description\": \"The time the operation was initiated.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the operation.\",\n      \"enum\": [\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"IN_PROGRESS\"\n      ],\n      \"example\": \"SUCCEEDED\"\n    },\n    \"statusMessage\": {\n      \"type\": \"string\",\n      \"description\": \"If the operation result is FAILED, this string contains a message explaining why.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/landing-zone-operation-detail-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: LandingZoneOperationDetail
---
