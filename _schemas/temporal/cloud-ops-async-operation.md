---
description: ''
layout: schema
name: AsyncOperation
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: checkDuration
  type: string
- description: ''
  name: operationType
  type: string
- description: ''
  name: startedTime
  type: string
- description: ''
  name: finishedTime
  type: string
- description: ''
  name: failureReason
  type: string
provider_name: Temporal
provider_slug: temporal
schema_file: json-schema/cloud-ops-async-operation-schema.json
slug: cloud-ops-async-operation
source_filename: cloud-ops-async-operation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AsyncOperation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"checkDuration\": {\n      \"type\": \"string\"\n    },\n    \"operationType\": {\n      \"type\": \"string\"\n    },\n    \"startedTime\": {\n      \"type\": \"string\"\n    },\n    \"finishedTime\": {\n      \"type\": \"string\"\n    },\n    \"failureReason\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/temporal/refs/heads/main/json-schema/cloud-ops-async-operation-schema.json
tags:
- ProCode_API_Composition
- Workflows
title: AsyncOperation
---
