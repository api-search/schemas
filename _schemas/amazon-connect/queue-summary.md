---
description: Contains summary information about a queue.
layout: schema
name: QueueSummary
properties_list:
- description: The identifier of the queue.
  name: Id
  type: string
- description: The Amazon Resource Name (ARN) of the queue.
  name: Arn
  type: string
- description: The name of the queue.
  name: Name
  type: string
- description: The type of queue.
  name: QueueType
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/queue-summary-schema.json
slug: queue-summary
source_filename: queue-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/queue-summary-schema.json\",\n  \"title\": \"QueueSummary\",\n  \"description\": \"Contains summary information about a queue.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Id\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the queue.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-55555EXAMPLE\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the queue.\"\n    },\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the queue.\",\n      \"example\": \"BasicQueue\"\n    },\n    \"QueueType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of queue.\",\n      \"enum\": [\n        \"STANDARD\",\n        \"AGENT\"\n      ],\n      \"example\": \"STANDARD\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/queue-summary-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: QueueSummary
---
