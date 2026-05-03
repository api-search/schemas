---
description: A content channel from the Reuters Connect API representing a curated feed of editorial content. Channels are organized by category (text, images, video, graphics) and subscription level, providing access to content from Reuters and partner sources.
layout: schema
name: Reuters Connect Channel
properties_list:
- description: The unique alias identifier for the channel, used as a reference in API calls to retrieve items from this channel.
  name: alias
  type: string
- description: A human-readable description of the channel content, explaining the editorial focus and type of content delivered.
  name: description
  type: string
- description: The content category of the channel, indicating the primary type of content delivered.
  name: category
  type: string
- description: The timestamp when the channel was last updated with new content, in ISO 8601 format.
  name: lastUpdated
  type: string
provider_name: Reuters
provider_slug: reuters
schema_file: json-schema/reuters-channel-schema.json
slug: reuters-channel
source_filename: reuters-channel-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/kinlane/reuters/json-schema/reuters-channel-schema.json\",\n  \"title\": \"Reuters Connect Channel\",\n  \"description\": \"A content channel from the Reuters Connect API representing a curated feed of editorial content. Channels are organized by category (text, images, video, graphics) and subscription level, providing access to content from Reuters and partner sources.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"alias\",\n    \"category\"\n  ],\n  \"properties\": {\n    \"alias\": {\n      \"type\": \"string\",\n      \"description\": \"The unique alias identifier for the channel, used as a reference in API calls to retrieve items from this channel.\",\n      \"examples\": [\n        \"OLDEN\",\n        \"RTRS_PIX\",\n        \"RTRS_VID\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of\
  \ the channel content, explaining the editorial focus and type of content delivered.\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The content category of the channel, indicating the primary type of content delivered.\",\n      \"enum\": [\n        \"TXT\",\n        \"PIX\",\n        \"VID\",\n        \"GFX\",\n        \"CMP\"\n      ]\n    },\n    \"lastUpdated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the channel was last updated with new content, in ISO 8601 format.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/reuters/refs/heads/main/json-schema/reuters-channel-schema.json
tags:
- Business
- Finance
- Journalism
- Media
- News
- Wire Service
title: Reuters Connect Channel
---
