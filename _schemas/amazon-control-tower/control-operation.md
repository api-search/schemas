---
description: An operation performed on a control.
layout: schema
name: ControlOperation
properties_list:
- description: The identifier of the control.
  name: controlIdentifier
  type: string
- description: The ARN of the enabled control.
  name: enabledControlIdentifier
  type: string
- description: ''
  name: endTime
  type: string
- description: The unique identifier of the operation.
  name: operationIdentifier
  type: string
- description: The type of operation.
  name: operationType
  type: string
- description: ''
  name: startTime
  type: string
- description: The status of the operation.
  name: status
  type: string
- description: An error message if the operation failed.
  name: statusMessage
  type: string
- description: The ARN of the organizational unit.
  name: targetIdentifier
  type: string
provider_name: Amazon Control Tower
provider_slug: amazon-control-tower
schema_file: json-schema/control-operation-schema.json
slug: control-operation
source_filename: control-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/control-operation-schema.json\",\n  \"title\": \"ControlOperation\",\n  \"description\": \"An operation performed on a control.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"controlIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the control.\"\n    },\n    \"enabledControlIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the enabled control.\"\n    },\n    \"endTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"operationIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the operation.\"\n    },\n    \"operationType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of operation.\",\n      \"enum\": [\n        \"ENABLE_CONTROL\"\
  ,\n        \"DISABLE_CONTROL\",\n        \"UPDATE_ENABLED_CONTROL\",\n        \"RESET_ENABLED_CONTROL\"\n      ]\n    },\n    \"startTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the operation.\",\n      \"enum\": [\n        \"SUCCEEDED\",\n        \"FAILED\",\n        \"IN_PROGRESS\"\n      ]\n    },\n    \"statusMessage\": {\n      \"type\": \"string\",\n      \"description\": \"An error message if the operation failed.\"\n    },\n    \"targetIdentifier\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the organizational unit.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-control-tower/refs/heads/main/json-schema/control-operation-schema.json
tags:
- Compliance
- Governance
- Landing Zone
- Multi-Account
- Security
- Controls
title: ControlOperation
---
