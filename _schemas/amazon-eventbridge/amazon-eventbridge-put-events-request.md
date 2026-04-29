---
description: PutEventsRequest schema from Amazon EventBridge API
layout: schema
name: PutEventsRequest
properties_list:
- description: The entry that defines an event in your system.
  name: Entries
  type: array
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-put-events-request-schema.json
slug: amazon-eventbridge-put-events-request
source_filename: amazon-eventbridge-put-events-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-put-events-request-schema.json\",\n  \"title\": \"PutEventsRequest\",\n  \"description\": \"PutEventsRequest schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Entries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Event\"\n      },\n      \"description\": \"The entry that defines an event in your system.\"\n    }\n  },\n  \"required\": [\n    \"Entries\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-put-events-request-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: PutEventsRequest
---
