---
description: CreateEventBusRequest schema from Amazon EventBridge API
layout: schema
name: CreateEventBusRequest
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: EventSourceName
  type: string
- description: ''
  name: Tags
  type: array
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-create-event-bus-request-schema.json
slug: amazon-eventbridge-create-event-bus-request
source_filename: amazon-eventbridge-create-event-bus-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-create-event-bus-request-schema.json\",\n  \"title\": \"CreateEventBusRequest\",\n  \"description\": \"CreateEventBusRequest schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\"\n    },\n    \"EventSourceName\": {\n      \"type\": \"string\"\n    },\n    \"Tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"Key\": {\n            \"type\": \"string\"\n          },\n          \"Value\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"Name\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-create-event-bus-request-schema.json
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: CreateEventBusRequest
---
