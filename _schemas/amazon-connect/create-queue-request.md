---
description: CreateQueueRequest schema from Amazon Connect Service API
layout: schema
name: CreateQueueRequest
properties_list:
- description: The name of the queue.
  name: Name
  type: string
- description: The description of the queue.
  name: Description
  type: string
- description: The identifier for the hours of operation.
  name: HoursOfOperationId
  type: string
- description: The maximum number of contacts that can be in the queue.
  name: MaxContacts
  type: integer
- description: ''
  name: OutboundCallerConfig
  type: object
- description: ''
  name: Tags
  type: object
provider_name: Amazon Connect
provider_slug: amazon-connect
schema_file: json-schema/create-queue-request-schema.json
slug: create-queue-request
source_filename: create-queue-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-queue-request-schema.json\",\n  \"title\": \"CreateQueueRequest\",\n  \"description\": \"CreateQueueRequest schema from Amazon Connect Service API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the queue.\",\n      \"example\": \"Support Queue\"\n    },\n    \"Description\": {\n      \"type\": \"string\",\n      \"description\": \"The description of the queue.\"\n    },\n    \"HoursOfOperationId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier for the hours of operation.\",\n      \"example\": \"a1b2c3d4-5678-90ab-cdef-66666EXAMPLE\"\n    },\n    \"MaxContacts\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of contacts that can be in the queue.\",\n     \
  \ \"example\": 100\n    },\n    \"OutboundCallerConfig\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"OutboundCallerIdName\": {\n          \"type\": \"string\"\n        },\n        \"OutboundCallerIdNumberId\": {\n          \"type\": \"string\"\n        },\n        \"OutboundFlowId\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"HoursOfOperationId\",\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-connect/refs/heads/main/json-schema/create-queue-request-schema.json
tags:
- Chat
- Contact Center
- Customer Service
- Voice
- AI
- Omnichannel
title: CreateQueueRequest
---
