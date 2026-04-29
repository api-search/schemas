---
description: Summary of a control operation.
layout: schema
name: ControlOperationSummary
properties_list:
- description: ''
  name: controlIdentifier
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
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/control-operation-summary-schema.json
slug: control-operation-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/control-operation-summary-schema.json\",\n  \"title\": \"ControlOperationSummary\",\n  \"description\": \"Summary of a control operation.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"controlIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"operationIdentifier\": {\n      \"type\": \"string\"\n    },\n    \"operationType\": {\n      \"type\": \"string\"\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/control-operation-summary-schema.json
tags:
- AWS
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: ControlOperationSummary
---
