---
description: ''
layout: schema
name: LiveStreamUpdateRequest
properties_list:
- description: Streaming URL (e.g., RTMP endpoint).
  name: stream_url
  type: string
- description: Stream key or name.
  name: stream_key
  type: string
- description: The live stream page URL where viewers can watch.
  name: page_url
  type: string
- description: The live stream resolution. Can be 720p or 1080p.
  name: resolution
  type: string
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-live-stream-update-request-schema.json
slug: zoom-meeting-live-stream-update-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveStreamUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"stream_url\": {\n      \"type\": \"string\",\n      \"description\": \"Streaming URL (e.g., RTMP endpoint).\"\n    },\n    \"stream_key\": {\n      \"type\": \"string\",\n      \"description\": \"Stream key or name.\"\n    },\n    \"page_url\": {\n      \"type\": \"string\",\n      \"description\": \"The live stream page URL where viewers can watch.\"\n    },\n    \"resolution\": {\n      \"type\": \"string\",\n      \"description\": \"The live stream resolution. Can be 720p or 1080p.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-live-stream-update-request-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: LiveStreamUpdateRequest
---
