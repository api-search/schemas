---
description: ''
layout: schema
name: Scheduler
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
- description: Timestamp when the scheduler was created.
  name: created_at
  type: string
provider_name: nOps
provider_slug: nops
schema_file: json-schema/nops-nops-scheduler-schema.json
slug: nops-nops-scheduler
source_filename: nops-nops-scheduler-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Scheduler\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique identifier of the scheduler.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the scheduler.\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the scheduler is currently enabled.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The associated nOps AWS Project ID.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Timestamp when the scheduler was created.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/json-schema/nops-nops-scheduler-schema.json
tags:
- Costs
- FinOps
title: Scheduler
---
