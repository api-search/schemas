---
description: Specifies a live video stream that has been ingested and distributed.
layout: schema
name: Stream
properties_list:
- description: ''
  name: channelArn
  type: object
- description: ''
  name: health
  type: object
- description: ''
  name: playbackUrl
  type: object
- description: ''
  name: startTime
  type: object
- description: ''
  name: state
  type: object
- description: ''
  name: streamId
  type: object
- description: ''
  name: viewerCount
  type: object
provider_name: Amazon Interactive Video Service
provider_slug: amazon-interactive-video-service
schema_file: json-schema/ivs-stream-schema.json
slug: ivs-stream
source_filename: ivs-stream-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-schema.json\",\n  \"title\": \"Stream\",\n  \"description\": \"Specifies a live video stream that has been ingested and distributed.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"channelArn\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/ChannelArn\"\n        },\n        {\n          \"description\": \"Channel ARN for the stream.\"\n        }\n      ]\n    },\n    \"health\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamHealth\"\n        },\n        {\n          \"description\": \"The stream\\u2019s health.\"\n        }\n      ]\n    },\n    \"playbackUrl\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/PlaybackURL\"\n        },\n        {\n          \"description\"\
  : \"URL of the master playlist, required by the video player to play the HLS stream.\"\n        }\n      ]\n    },\n    \"startTime\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamStartTime\"\n        },\n        {\n          \"description\": \"Time of the stream\\u2019s start. This is an ISO 8601 timestamp; <i>note that this is returned as a string</i>.\"\n        }\n      ]\n    },\n    \"state\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamState\"\n        },\n        {\n          \"description\": \"The stream\\u2019s state. Do not rely on the <code>OFFLINE</code> state, as the API may not return it; instead, a \\\"NotBroadcasting\\\" error will indicate that the stream is not live.\"\n        }\n      ]\n    },\n    \"streamId\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamId\"\n        },\n        {\n          \"description\": \"Unique identifier for a live or previously\
  \ live stream in the specified channel.\"\n        }\n      ]\n    },\n    \"viewerCount\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/StreamViewerCount\"\n        },\n        {\n          \"description\": \"A count of concurrent views of the stream. Typically, a new view appears in <code>viewerCount</code> within 15 seconds of when video playback starts and a view is removed from <code>viewerCount</code> within 1 minute of when video playback ends. A value of -1 indicates that the request timed out; in this case, retry.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-interactive-video-service/refs/heads/main/json-schema/ivs-stream-schema.json
tags:
- AWS
- Live Streaming
- Media
- Video
- Real-Time
title: Stream
---
