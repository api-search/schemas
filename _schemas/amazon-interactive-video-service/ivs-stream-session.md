---
description: Object that captures the Amazon IVS configuration that the customer provisioned, the ingest configurations that the broadcaster used, and the most recent Amazon IVS stream events it encountered.
layout: schema
name: StreamSession
properties_list:
- description: ''
  name: channel
  type: object
- description: ''
  name: endTime
  type: object
- description: ''
  name: ingestConfiguration
  type: object
- description: ''
  name: recordingConfiguration
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: streamId
  type: object
- description: ''
  name: truncatedEvents
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-stream-session-schema.json
slug: ivs-stream-session
source_filename: ivs-stream-session-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-session-schema.json\",\n  \"title\": \"StreamSession\",\n  \"description\": \"Object that captures the Amazon IVS configuration that the customer provisioned, the ingest configurations that the broadcaster used, and the most recent Amazon IVS stream events it encountered.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channel\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Channel\"\n        },\n        {\n          \"description\": \"The properties of the channel at the time of going live.\"\n        }\n      ]\n    },\n    \"endTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"Time when the channel went offline. This is an ISO 8601 timestamp;\
  \ <i>note that this is returned as a string</i>. For live streams, this is <code>NULL</code>.\"\n        }\n      ]\n    },\n    \"ingestConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/IngestConfiguration\"\n        },\n        {\n          \"description\": \"The properties of the incoming RTMP stream for the stream.\"\n        }\n      ]\n    },\n    \"recordingConfiguration\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/RecordingConfiguration\"\n        },\n        {\n          \"description\": \"The properties of recording the live stream.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/Time\"\n        },\n        {\n          \"description\": \"Time when the channel went live. This is an ISO 8601 timestamp; <i>note that this is returned as a string</i>.\"\n        }\n      ]\n    },\n    \"streamId\": {\n      \"allOf\": [\n \
  \       {\n          \"$ref\": \"#/components/schemas/StreamId\"\n        },\n        {\n          \"description\": \"Unique identifier for a live or previously live stream in the specified channel.\"\n        }\n      ]\n    },\n    \"truncatedEvents\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamEvents\"\n        },\n        {\n          \"description\": \"List of Amazon IVS events that the stream encountered. The list is sorted by most recent events and contains up to 500 events. For Amazon IVS events, see <a href=\\\"https://docs.aws.amazon.com/ivs/latest/userguide/eventbridge.html\\\">Using Amazon EventBridge with Amazon IVS</a>.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-session-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: StreamSession
---
