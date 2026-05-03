---
description: A Zesty.io media bin is a top-level container for organizing media files and groups within the Media Manager service.
layout: schema
name: Zesty Media Bin
properties_list:
- description: The Zesty Universal Identifier for the bin.
  name: ZUID
  type: string
- description: The name of the media bin.
  name: name
  type: string
- description: Timestamp when the bin was created.
  name: createdAt
  type: string
- description: Timestamp when the bin was last updated.
  name: updatedAt
  type: string
provider_name: Zesty
provider_slug: zesty
schema_file: json-schema/media-bin.json
slug: media-bin
source_filename: media-bin.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/zesty/blob/main/json-schema/media-bin.json\",\n  \"title\": \"Zesty Media Bin\",\n  \"description\": \"A Zesty.io media bin is a top-level container for organizing media files and groups within the Media Manager service.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"ZUID\": {\n      \"type\": \"string\",\n      \"description\": \"The Zesty Universal Identifier for the bin.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the media bin.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the bin was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the bin was last updated.\"\n    }\n  },\n  \"required\": [\"ZUID\", \"name\"]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zesty/refs/heads/main/json-schema/media-bin.json
tags:
- CMS
- Composable
- Content Management
- Headless CMS
- Media
title: Zesty Media Bin
---
