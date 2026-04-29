---
description: Basic details about a live stream including its title, description, and channel association.
layout: schema
name: LiveStreamSnippet
properties_list:
- description: The ID of the channel to which this stream is affiliated.
  name: channelId
  type: string
- description: The stream's title. The value must be between 1 and 128 characters long.
  name: title
  type: string
- description: The stream's description. The value cannot be longer than 10000 characters.
  name: description
  type: string
- description: The date and time that the stream was created.
  name: publishedAt
  type: string
- description: Indicates whether this stream is the default stream.
  name: isDefaultStream
  type: boolean
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-live-live-stream-snippet-schema.json
slug: youtube-live-live-stream-snippet
source_filename: youtube-live-live-stream-snippet-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Basic details about a live stream including its title, description, and channel association.\",\n  \"properties\": {\n    \"channelId\": {\n      \"type\": \"string\",\n      \"description\": \"The ID of the channel to which this stream is affiliated.\",\n      \"example\": \"500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The stream's title. The value must be between 1 and 128 characters long.\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The stream's description. The value cannot be longer than 10000 characters.\",\n      \"example\": \"A sample description for this resource.\"\n    },\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the stream was created.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n  \
  \  \"isDefaultStream\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether this stream is the default stream.\",\n      \"example\": true\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"LiveStreamSnippet\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-live-streaming-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-live-live-stream-snippet-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: LiveStreamSnippet
---
