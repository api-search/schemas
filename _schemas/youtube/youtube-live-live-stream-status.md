---
description: Status information about a live stream including its stream status and health status.
layout: schema
name: LiveStreamStatus
properties_list:
- description: The stream's current status.
  name: streamStatus
  type: string
- description: The health status of the stream.
  name: healthStatus
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-stream-status-schema.json
slug: youtube-live-live-stream-status
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Status information about a live stream including its stream status and health status.\",\n  \"properties\": {\n    \"streamStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The stream's current status.\",\n      \"example\": \"active\",\n      \"enum\": [\n        \"active\",\n        \"created\",\n        \"error\",\n        \"inactive\",\n        \"ready\"\n      ]\n    },\n    \"healthStatus\": {\n      \"type\": \"object\",\n      \"description\": \"The health status of the stream.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The status code of this stream.\",\n          \"enum\": [\n            \"bad\",\n            \"good\",\n            \"noData\",\n            \"ok\",\n            \"revoked\"\n          ]\n        },\n        \"lastUpdateTimeSeconds\": {\n          \"type\": \"integer\",\n     \
  \     \"description\": \"The last time this status was updated, as a Unix timestamp.\",\n          \"format\": \"int64\"\n        },\n        \"configurationIssues\": {\n          \"type\": \"array\",\n          \"description\": \"The configurations issues on this stream.\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"The kind of error happening.\"\n              },\n              \"severity\": {\n                \"type\": \"string\",\n                \"description\": \"How severe this issue is to the stream.\",\n                \"enum\": [\n                  \"error\",\n                  \"info\",\n                  \"warning\"\n                ]\n              },\n              \"reason\": {\n                \"type\": \"string\",\n                \"description\": \"The short-form reason for this issue.\"\n              },\n              \"\
  description\": {\n                \"type\": \"string\",\n                \"description\": \"The long-form description of the issue and how to resolve it.\"\n              }\n            }\n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveStreamStatus\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-stream-status-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveStreamStatus
---
