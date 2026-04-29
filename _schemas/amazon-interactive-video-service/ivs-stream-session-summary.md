---
description: Summary information about a stream session.
layout: schema
name: StreamSessionSummary
properties_list:
- description: ''
  name: endTime
  type: object
- description: ''
  name: hasErrorEvent
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: streamId
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-stream-session-summary-schema.json
slug: ivs-stream-session-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-session-summary-schema.json\",\n  \"title\": \"StreamSessionSummary\",\n  \"description\": \"Summary information about a stream session.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"Time when the channel went offline. This is an ISO 8601 timestamp; <i>note that this is returned as a string</i>. For live streams, this is <code>NULL</code>.\"\n        }\n      ]\n    },\n    \"hasErrorEvent\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Boolean\"\n        },\n        {\n          \"description\": \"If <code>true</code>, this stream encountered a quota breach or failure.\"\n        }\n   \
  \   ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"Time when the channel went live. This is an ISO 8601 timestamp; <i>note that this is returned as a string</i>.\"\n        }\n      ]\n    },\n    \"streamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamId\"\n        },\n        {\n          \"description\": \"Unique identifier for a live or previously live stream in the specified channel.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-session-summary-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: StreamSessionSummary
---
