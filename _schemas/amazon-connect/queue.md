---
description: Contains information about a queue.
layout: schema
name: Queue
properties_list:
- description: The name of the queue.
  name: Name
  type: string
- description: The Amazon Resource Name (ARN) for the queue.
  name: QueueArn
  type: string
- description: The identifier for the queue.
  name: QueueId
  type: string
- description: The description of the queue.
  name: Description
  type: string
- description: ''
  name: OutboundCallerConfig
  type: object
- description: The identifier for the hours of operation.
  name: HoursOfOperationId
  type: string
- description: The maximum number of contacts that can be in the queue before it is considered full.
  name: MaxContacts
  type: integer
- description: The status of the queue.
  name: Status
  type: string
- description: ''
  name: Tags
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/queue-schema.json
slug: queue
source_filename: queue-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/queue-schema.json\",\n  \"title\": \"Queue\",\n  \"description\": \"Contains information about a queue.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the queue.\",\n      \"example\": \"BasicQueue\"\n    },\n    \"QueueArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) for the queue.\"\n    },\n    \"QueueId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the queue.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-55555EXAMPLE\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the queue.\"\n    },\n    \"OutboundCallerConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n   \
  \     \"OutboundCallerIdName\": {\n          \"type\": \"string\"\n        },\n        \"OutboundCallerIdNumberId\": {\n          \"type\": \"string\"\n        },\n        \"OutboundFlowId\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"HoursOfOperationId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the hours of operation.\"\n    },\n    \"MaxContacts\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of contacts that can be in the queue before it is considered full.\",\n      \"example\": 100\n    },\n    \"Status\": {\n      \"type\": \"string\",\n      \"description\": \"The status of the queue.\",\n      \"enum\": [\n        \"ENABLED\",\n        \"DISABLED\"\n      ],\n      \"example\": \"ENABLED\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/queue-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: Queue
---
