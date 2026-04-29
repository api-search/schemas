---
description: A Scheduler automates resource management tasks such as starting and stopping non-production workloads on a defined schedule to reduce costs.
layout: schema
name: nOps Scheduler
properties_list:
- description: The unique identifier of the scheduler.
  name: id
  type: integer
- description: Name of the scheduler.
  name: name
  type: string
- description: Whether the scheduler is currently enabled.
  name: enabled
  type: boolean
- description: The associated nOps AWS Project ID.
  name: project_id
  type: integer
- description: Schedule configuration defining when the scheduler runs.
  name: schedule
  type: object
- description: List of resources managed by this scheduler.
  name: resources
  type: array
- description: Timestamp when the scheduler was created.
  name: created_at
  type: string
provider_name: nOps
provider_slug: nops
schema_file: json-schema/scheduler.json
slug: scheduler
source_filename: scheduler.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/nops/blob/main/json-schema/scheduler.json\",\n  \"title\": \"nOps Scheduler\",\n  \"description\": \"A Scheduler automates resource management tasks such as starting and stopping non-production workloads on a defined schedule to reduce costs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the scheduler.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the scheduler.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the scheduler is currently enabled.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The associated nOps AWS Project ID.\"\n    },\n    \"schedule\": {\n      \"type\": \"object\",\n      \"description\": \"Schedule configuration\
  \ defining when the scheduler runs.\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"List of resources managed by this scheduler.\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the scheduler was created.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/json-schema/scheduler.json
tags:
- Costs
- FinOps
title: nOps Scheduler
---
