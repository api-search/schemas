---
description: A job queue within a render farm that organizes and schedules rendering jobs.
layout: schema
name: Queue
properties_list:
- description: The unique identifier of the queue
  name: queueId
  type: string
- description: ''
  name: farmId
  type: string
- description: ''
  name: displayName
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: createdAt
  type: string
provider_name: Amazon Deadline Cloud
provider_slug: amazon-deadline-cloud
schema_file: json-schema/queue-schema.json
slug: queue
source_filename: queue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/amazon-deadline-cloud/json-schema/queue-schema.json\",\n  \"title\": \"Queue\",\n  \"description\": \"A job queue within a render farm that organizes and schedules rendering jobs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"queueId\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the queue\"\n    },\n    \"farmId\": {\n      \"type\": \"string\"\n    },\n    \"displayName\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ACTIVE\",\n        \"SCHEDULING\",\n        \"SCHEDULING_BLOCKED\"\n      ]\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-deadline-cloud/refs/heads/main/json-schema/queue-schema.json
tags:
- AWS
- Compute
- Media
- Rendering
- Visual Effects
title: Queue
---
