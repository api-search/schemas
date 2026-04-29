---
description: PutEventsResponse schema from Amazon EventBridge API
layout: schema
name: PutEventsResponse
properties_list:
- description: The number of failed entries.
  name: FailedEntryCount
  type: integer
- description: ''
  name: Entries
  type: array
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-put-events-response-schema.json
slug: amazon-eventbridge-put-events-response
source_filename: amazon-eventbridge-put-events-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-put-events-response-schema.json\",\n  \"title\": \"PutEventsResponse\",\n  \"description\": \"PutEventsResponse schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedEntryCount\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of failed entries.\"\n    },\n    \"Entries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"EventId\": {\n            \"type\": \"string\"\n          },\n          \"ErrorCode\": {\n            \"type\": \"string\"\n          },\n          \"ErrorMessage\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-put-events-response-schema.json
tags:
- Amazon Web Services
- AWS
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: PutEventsResponse
---
