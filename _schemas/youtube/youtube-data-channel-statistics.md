---
description: Statistics about a YouTube channel.
layout: schema
name: ChannelStatistics
properties_list:
- description: The number of times the channel has been viewed.
  name: viewCount
  type: string
- description: The number of subscribers that the channel has.
  name: subscriberCount
  type: string
- description: Indicates whether the channel's subscriber count is publicly visible.
  name: hiddenSubscriberCount
  type: boolean
- description: The number of public videos uploaded to the channel.
  name: videoCount
  type: string
provider_name: Youtube
provider_slug: youtube
schema_file: json-schema/youtube-data-channel-statistics-schema.json
slug: youtube-data-channel-statistics
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Statistics about a YouTube channel.\",\n  \"properties\": {\n    \"viewCount\": {\n      \"type\": \"string\",\n      \"description\": \"The number of times the channel has been viewed.\",\n      \"example\": 42\n    },\n    \"subscriberCount\": {\n      \"type\": \"string\",\n      \"description\": \"The number of subscribers that the channel has.\",\n      \"example\": 42\n    },\n    \"hiddenSubscriberCount\": {\n      \"type\": \"boolean\",\n      \"description\": \"Indicates whether the channel's subscriber count is publicly visible.\",\n      \"example\": 42\n    },\n    \"videoCount\": {\n      \"type\": \"string\",\n      \"description\": \"The number of public videos uploaded to the channel.\",\n      \"example\": 42\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ChannelStatistics\",\n  \"x-schema-source\": \"openapi\",\n  \"x-source-url\": \"openapi/youtube-data-api-openapi.yml\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/youtube/refs/heads/main/json-schema/youtube-data-channel-statistics-schema.json
tags:
- Google
- Media
- Social
- Streaming
- Video
- Videos
title: ChannelStatistics
---
