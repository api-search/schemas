---
description: EventBus schema from Amazon EventBridge API
layout: schema
name: EventBus
properties_list:
- description: The name of the event bus.
  name: Name
  type: string
- description: The ARN of the event bus.
  name: Arn
  type: string
- description: The permissions policy of the event bus.
  name: Policy
  type: string
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-event-bus-schema.json
slug: amazon-eventbridge-event-bus
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-event-bus-schema.json\",\n  \"title\": \"EventBus\",\n  \"description\": \"EventBus schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the event bus.\"\n    },\n    \"Arn\": {\n      \"type\": \"string\",\n      \"description\": \"The ARN of the event bus.\"\n    },\n    \"Policy\": {\n      \"type\": \"string\",\n      \"description\": \"The permissions policy of the event bus.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-event-bus-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: EventBus
---
