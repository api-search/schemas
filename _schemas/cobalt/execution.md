---
description: A workflow execution record within the Cobalt embedded integration platform.
layout: schema
name: Execution
properties_list:
- description: Execution ID.
  name: _id
  type: string
- description: The workflow that was executed.
  name: workflow_id
  type: string
- description: The linked account ID.
  name: linked_account_id
  type: string
- description: Execution status.
  name: status
  type: string
- description: Execution start timestamp.
  name: started_at
  type: string
- description: Execution completion timestamp.
  name: completed_at
  type: string
- description: Execution logs.
  name: logs
  type: array
provider_name: Cobalt
provider_slug: cobalt
schema_file: json-schema/execution.json
slug: execution
source_filename: execution.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/execution.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Execution\",\n  \"description\": \"A workflow execution record within the Cobalt embedded integration platform.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"_id\": {\n      \"type\": \"string\",\n      \"description\": \"Execution ID.\"\n    },\n    \"workflow_id\": {\n      \"type\": \"string\",\n      \"description\": \"The workflow that was executed.\"\n    },\n    \"linked_account_id\": {\n      \"type\": \"string\",\n      \"description\": \"The linked account ID.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"pending\",\n        \"running\",\n        \"completed\",\n        \"failed\"\n      ],\n      \"description\": \"Execution status.\"\n    },\n    \"started_at\": {\n      \"type\": \"string\",\n      \"format\": \"\
  date-time\",\n      \"description\": \"Execution start timestamp.\"\n    },\n    \"completed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Execution completion timestamp.\"\n    },\n    \"logs\": {\n      \"type\": \"array\",\n      \"description\": \"Execution logs.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/cobalt/refs/heads/main/json-schema/execution.json
tags:
- Automation
- Embedded iPaaS
- Integrations
title: Execution
---
