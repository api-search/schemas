---
description: An operation performed on a baseline.
layout: schema
name: BaselineOperation
properties_list:
- description: ''
  name: endTime
  type: string
- description: ''
  name: operationIdentifier
  type: string
- description: ''
  name: operationType
  type: string
- description: ''
  name: startTime
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: statusMessage
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/baseline-operation-schema.json
slug: baseline-operation
source_filename: baseline-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/baseline-operation-schema.json\",\n  \"title\": \"BaselineOperation\",\n  \"description\": \"An operation performed on a baseline.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"operationIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"operationType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ENABLE_BASELINE\",\n        \"DISABLE_BASELINE\",\n        \"UPDATE_ENABLED_BASELINE\",\n        \"RESET_ENABLED_BASELINE\"\n      ]\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"IN_PROGRESS\"\n      ]\n    },\n\
  \    \"statusMessage\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/baseline-operation-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: BaselineOperation
---
