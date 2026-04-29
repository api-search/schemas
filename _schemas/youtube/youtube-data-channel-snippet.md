---
description: Basic details about a channel, including its title, description, and thumbnails.
layout: schema
name: ChannelSnippet
properties_list:
- description: The channel title.
  name: title
  type: string
- description: The channel description.
  name: description
  type: string
- description: The channel's custom URL.
  name: customUrl
  type: string
- description: The date and time that the channel was created.
  name: publishedAt
  type: string
- description: A map of thumbnail images associated with the channel.
  name: thumbnails
  type: object
- description: The country with which the channel is associated.
  name: country
  type: string
- description: The snippet.localized object contains a localized title and description for the channel.
  name: localized
  type: object
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-channel-snippet-schema.json
slug: youtube-data-channel-snippet
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Basic details about a channel, including its title, description, and thumbnails.\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"The channel title.\",\n      \"example\": \"Example Title\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"The channel description.\",\n      \"example\": \"A sample description for this resource.\"\n    },\n    \"customUrl\": {\n      \"type\": \"string\",\n      \"description\": \"The channel's custom URL.\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"publishedAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time that the channel was created.\",\n      \"example\": \"2026-01-15T10:30:00Z\",\n      \"format\": \"date-time\"\n    },\n    \"thumbnails\": {\n      \"type\": \"object\",\n      \"description\": \"A map of thumbnail images associated with the channel.\"\
  ,\n      \"example\": \"example_value\"\n    },\n    \"country\": {\n      \"type\": \"string\",\n      \"description\": \"The country with which the channel is associated.\",\n      \"example\": 42\n    },\n    \"localized\": {\n      \"type\": \"object\",\n      \"description\": \"The snippet.localized object contains a localized title and description for the channel.\",\n      \"example\": \"example_value\",\n      \"properties\": {\n        \"title\": {\n          \"type\": \"string\",\n          \"description\": \"The localized channel title.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"The localized channel description.\"\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChannelSnippet\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-channel-snippet-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: ChannelSnippet
---
