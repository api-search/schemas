---
description: A compute worker instance in a Deadline Cloud fleet executing rendering tasks.
layout: schema
name: Worker
properties_list:
- description: The unique identifier of the worker
  name: workerId
  type: string
- description: ''
  name: fleetId
  type: string
- description: ''
  name: farmId
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/worker-schema.json
slug: worker
source_filename: worker-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/worker-schema.json\",\n  \"title\": \"Worker\",\n  \"description\": \"A compute worker instance in a Deadline Cloud fleet executing rendering tasks.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"workerId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the worker\"\n    },\n    \"fleetId\": {\n      \"type\": \"string\"\n    },\n    \"farmId\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/worker-schema.json
tags:
- Compute
- Media
- Rendering
- Visual Effects
title: Worker
---
