---
description: Object specifying a stream’s events. For a list of events, see <a href="https://docs.aws.amazon.com/ivs/latest/userguide/eventbridge.html">Using Amazon EventBridge with Amazon IVS</a>.
layout: schema
name: StreamEvent
properties_list:
- description: ''
  name: eventTime
  type: object
- description: ''
  name: name
  type: object
- description: ''
  name: type
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-stream-event-schema.json
slug: ivs-stream-event
source_filename: ivs-stream-event-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-event-schema.json\",\n  \"title\": \"StreamEvent\",\n  \"description\": \"Object specifying a stream\\u2019s events. For a list of events, see <a href=\\\"https://docs.aws.amazon.com/ivs/latest/userguide/eventbridge.html\\\">Using Amazon EventBridge with Amazon IVS</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"Time when the event occurred. This is an ISO 8601 timestamp; <i>note that this is returned as a string</i>.\"\n        }\n      ]\n    },\n    \"name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Name that identifies\
  \ the stream event within a <code>type</code>.\"\n        }\n      ]\n    },\n    \"type\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/String\"\n        },\n        {\n          \"description\": \"Logical group for certain events.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-event-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: StreamEvent
---
