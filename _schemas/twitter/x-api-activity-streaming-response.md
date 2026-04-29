---
description: An activity event or error that can be returned by the x activity streaming API.
layout: schema
name: ActivityStreamingResponse
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: errors
  type: array
provider_name: X (Twitter)
provider_slug: twitter
schema_file: json-schema/x-api-activity-streaming-response-schema.json
slug: x-api-activity-streaming-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-activity-streaming-response-schema.json\",\n  \"title\": \"ActivityStreamingResponse\",\n  \"description\": \"An activity event or error that can be returned by the x activity streaming API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"event_type\": {\n          \"type\": \"string\"\n        },\n        \"event_uuid\": {\n          \"$ref\": \"#/components/schemas/ActivityEventId\"\n        },\n        \"filter\": {\n          \"$ref\": \"#/components/schemas/ActivitySubscriptionFilter\"\n        },\n        \"payload\": {\n          \"$ref\": \"#/components/schemas/ActivityStreamingResponsePayload\"\n        },\n        \"tag\": {\n          \"type\": \"string\"\n        }\n      }\n    },\n    \"errors\": {\n      \"\
  type\": \"array\",\n      \"minItems\": 1,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Problem\"\n      },\n      \"example\": []\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/twitter/refs/heads/main/json-schema/x-api-activity-streaming-response-schema.json
tags:
- Social Media
- Microblogging
- Real-Time Data
- Streaming
- Advertising
- Content
title: ActivityStreamingResponse
---
