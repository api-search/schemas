---
description: ''
layout: schema
name: SchedulerCreateRequest
properties_list:
- description: Name of the scheduler.
  name: name
  type: string
- description: The nOps AWS Project ID to associate with.
  name: project_id
  type: integer
- description: Schedule configuration for the scheduler.
  name: schedule
  type: object
- description: List of resources to manage with this scheduler.
  name: resources
  type: array
provider_name: nOps
provider_slug: nops
schema_file: json-schema/nops-nops-scheduler-create-request-schema.json
slug: nops-nops-scheduler-create-request
source_filename: nops-nops-scheduler-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SchedulerCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the scheduler.\"\n    },\n    \"project_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The nOps AWS Project ID to associate with.\"\n    },\n    \"schedule\": {\n      \"type\": \"object\",\n      \"description\": \"Schedule configuration for the scheduler.\"\n    },\n    \"resources\": {\n      \"type\": \"array\",\n      \"description\": \"List of resources to manage with this scheduler.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/nops/refs/heads/main/json-schema/nops-nops-scheduler-create-request-schema.json
tags:
- Costs
- FinOps
title: SchedulerCreateRequest
---
