---
description: Status of a long-running operation such as an application package installation.
layout: schema
name: OperationStatus
properties_list:
- description: The unique identifier of the operation.
  name: id
  type: string
- description: The current status of the operation.
  name: status
  type: string
- description: The timestamp when the operation was created.
  name: createdDateTime
  type: string
- description: The timestamp of the last status update.
  name: lastActionDateTime
  type: string
- description: Error details if the operation failed.
  name: error
  type: '[''object'', ''null'']'
provider_name: Microsoft Power Platform APIs
provider_slug: power-platform
schema_file: json-schema/power-platform-operation-status-schema.json
slug: power-platform-operation-status
source_filename: power-platform-operation-status-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OperationStatus\",\n  \"type\": \"object\",\n  \"description\": \"Status of a long-running operation such as an application package installation.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the operation.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the operation.\"\n    },\n    \"createdDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp when the operation was created.\"\n    },\n    \"lastActionDateTime\": {\n      \"type\": \"string\",\n      \"description\": \"The timestamp of the last status update.\"\n    },\n    \"error\": {\n      \"type\": \"['object', 'null']\",\n      \"description\": \"Error details if the operation failed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/power-platform/refs/heads/main/json-schema/power-platform-operation-status-schema.json
tags:
- Business Applications
- Copilot Studio
- Dataverse
- Low-Code
- Microsoft
- No-Code
- Power Pages
- Power Platform
title: OperationStatus
---
