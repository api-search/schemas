---
description: List of video clips.
layout: schema
name: VideoClipList
properties_list:
- description: Array of video clips.
  name: clips
  type: array
provider_name: ADT
provider_slug: adt
schema_file: json-schema/platform-api-video-clip-list-schema.json
slug: platform-api-video-clip-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-video-clip-list-schema.json\",\n  \"title\": \"VideoClipList\",\n  \"description\": \"List of video clips.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"clips\": {\n      \"type\": \"array\",\n      \"description\": \"Array of video clips.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"A recorded video clip from a security camera.\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\",\n            \"description\": \"Unique identifier of the video clip.\",\n            \"example\": \"clip-001\"\n          },\n          \"cameraId\": {\n            \"type\": \"string\",\n            \"description\": \"ID of the camera that recorded the clip.\",\n            \"example\": \"dev-cam-001\"\n          },\n          \"startTime\": {\n\
  \            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"Start timestamp of the recording.\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"endTime\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\",\n            \"description\": \"End timestamp of the recording.\",\n            \"example\": \"2025-03-15T14:31:00Z\"\n          },\n          \"trigger\": {\n            \"type\": \"string\",\n            \"description\": \"What triggered the recording.\",\n            \"enum\": [\n              \"motion\",\n              \"alarm\",\n              \"manual\",\n              \"schedule\"\n            ],\n            \"example\": \"motion\"\n          },\n          \"downloadUrl\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"Pre-signed URL to download the video clip.\",\n            \"example\": \"https://media.adt.com/clips/clip-001.mp4\"\
  \n          },\n          \"thumbnailUrl\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL of the clip thumbnail image.\",\n            \"example\": \"https://media.adt.com/thumbnails/clip-001.jpg\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/json-schema/platform-api-video-clip-list-schema.json
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
title: VideoClipList
---
