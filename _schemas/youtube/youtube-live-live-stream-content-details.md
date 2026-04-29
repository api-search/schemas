---
description: Detailed settings for a live stream including the stream key and ingestion settings.
layout: schema
name: LiveStreamContentDetails
properties_list:
- description: The ID of the live broadcast to which this stream is bound.
  name: boundBroadcastId
  type: string
- description: Indicates whether the stream is reusable, which means that it can be bound to multiple broadcasts.
  name: isReusable
  type: boolean
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-stream-content-details-schema.json
slug: youtube-live-live-stream-content-details
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed settings for a live stream including the stream key and ingestion settings.\",\n  \"properties\": {\n    \"boundBroadcastId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the live broadcast to which this stream is bound.\",\n      \"example\": \"500123\"\n    },\n    \"isReusable\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the stream is reusable, which means that it can be bound to multiple broadcasts.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveStreamContentDetails\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-stream-content-details-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveStreamContentDetails
---
