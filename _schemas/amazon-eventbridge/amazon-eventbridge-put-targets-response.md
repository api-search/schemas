---
description: PutTargetsResponse schema from Amazon EventBridge API
layout: schema
name: PutTargetsResponse
properties_list:
- description: ''
  name: FailedEntryCount
  type: integer
- description: ''
  name: FailedEntries
  type: array
provider_name: Amazon EventBridge
provider_slug: amazon-eventbridge
schema_file: json-schema/amazon-eventbridge-put-targets-response-schema.json
slug: amazon-eventbridge-put-targets-response
source_filename: amazon-eventbridge-put-targets-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-put-targets-response-schema.json\",\n  \"title\": \"PutTargetsResponse\",\n  \"description\": \"PutTargetsResponse schema from Amazon EventBridge API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"FailedEntryCount\": {\n      \"type\": \"integer\"\n    },\n    \"FailedEntries\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"TargetId\": {\n            \"type\": \"string\"\n          },\n          \"ErrorCode\": {\n            \"type\": \"string\"\n          },\n          \"ErrorMessage\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-eventbridge/refs/heads/main/json-schema/amazon-eventbridge-put-targets-response-schema.json
tags:
- Amazon Web Services
- Event Bus
- Event-Driven
- Events
- Integration
- Serverless
title: PutTargetsResponse
---
