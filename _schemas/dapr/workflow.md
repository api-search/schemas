---
description: Represents the status and details of a Dapr workflow instance, including its runtime status, creation time, and associated properties.
layout: schema
name: Dapr Workflow
properties_list:
- description: The unique identifier of the workflow instance.
  name: instanceID
  type: string
- description: The name of the workflow definition.
  name: workflowName
  type: string
- description: Timestamp of when the workflow instance was created.
  name: createdAt
  type: string
- description: Timestamp of when the workflow instance was last updated.
  name: lastUpdatedAt
  type: string
- description: The current runtime status of the workflow instance.
  name: runtimeStatus
  type: string
- description: Additional workflow properties as key/value pairs.
  name: properties
  type: object
provider_name: Dapr
provider_slug: dapr
schema_file: json-schema/workflow.json
slug: workflow
source_filename: workflow.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/dapr/blob/main/json-schema/workflow.json\",\n  \"title\": \"Dapr Workflow\",\n  \"description\": \"Represents the status and details of a Dapr workflow instance, including its runtime status, creation time, and associated properties.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"instanceID\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the workflow instance.\"\n    },\n    \"workflowName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the workflow definition.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the workflow instance was created.\"\n    },\n    \"lastUpdatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of when the workflow instance\
  \ was last updated.\"\n    },\n    \"runtimeStatus\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RUNNING\",\n        \"COMPLETED\",\n        \"FAILED\",\n        \"TERMINATED\",\n        \"PENDING\",\n        \"SUSPENDED\"\n      ],\n      \"description\": \"The current runtime status of the workflow instance.\"\n    },\n    \"properties\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional workflow properties as key/value pairs.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/dapr/refs/heads/main/json-schema/workflow.json
tags:
- Distributed Systems
- Microservices
- Platform
- Pub/Sub
- State Management
- Workflows
title: Dapr Workflow
---
