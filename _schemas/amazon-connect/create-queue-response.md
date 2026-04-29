---
description: CreateQueueResponse schema from Amazon Connect Service API
layout: schema
name: CreateQueueResponse
properties_list:
- description: The Amazon Resource Name (ARN) of the queue.
  name: QueueArn
  type: string
- description: The identifier for the queue.
  name: QueueId
  type: string
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-queue-response-schema.json
slug: create-queue-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-queue-response-schema.json\",\n  \"title\": \"CreateQueueResponse\",\n  \"description\": \"CreateQueueResponse schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"QueueArn\": {\n      \"type\": \"string\",\n      \"description\": \"The Amazon Resource Name (ARN) of the queue.\"\n    },\n    \"QueueId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the queue.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-55555EXAMPLE\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-queue-response-schema.json
tags:
- AWS
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateQueueResponse
---
