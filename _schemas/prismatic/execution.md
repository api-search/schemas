---
description: An execution represents a single run of an instance flow, including its status, logs, step results, and timing information.
layout: schema
name: Prismatic Execution
properties_list:
- description: Unique identifier for the execution
  name: id
  type: string
- description: Current status of the execution
  name: status
  type: string
- description: The instance this execution belongs to
  name: instance
  type: object
- description: The flow that was executed
  name: flow
  type: object
- description: Results from each step in the execution
  name: stepResults
  type: array
- description: Number of retry attempts for this execution
  name: retryAttempts
  type: integer
- description: ID of the original execution if this is a retry
  name: retryForExecutionId
  type: string
- description: Timestamp when the execution started
  name: startedAt
  type: string
- description: Timestamp when the execution ended
  name: endedAt
  type: string
provider_name: Prismatic
provider_slug: prismatic
schema_file: json-schema/execution.json
slug: execution
source_filename: execution.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/execution.json\",\n  \"title\": \"Prismatic Execution\",\n  \"description\": \"An execution represents a single run of an instance flow, including its status, logs, step results, and timing information.\",\n  \"type\": \"object\",\n  \"required\": [\"id\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the execution\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\"pending\", \"running\", \"completed\", \"failed\", \"canceled\"],\n      \"description\": \"Current status of the execution\"\n    },\n    \"instance\": {\n      \"$ref\": \"instance.json\",\n      \"description\": \"The instance this execution belongs to\"\n    },\n    \"flow\": {\n      \"$ref\": \"flow.json\",\n      \"description\": \"The flow that was\
  \ executed\"\n    },\n    \"stepResults\": {\n      \"type\": \"array\",\n      \"description\": \"Results from each step in the execution\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"stepName\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\"pending\", \"running\", \"completed\", \"failed\"]\n          },\n          \"startedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"endedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"retryAttempts\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of retry attempts for this execution\"\n    },\n    \"retryForExecutionId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the original execution if this is a retry\"\n    },\n    \"startedAt\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the execution started\"\n    },\n    \"endedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the execution ended\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/prismatic/refs/heads/main/json-schema/execution.json
tags:
- Embedded iPaaS
- Integrations
- Workflows
title: Prismatic Execution
---
