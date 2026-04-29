---
description: Represents a media asset in the Camtasia asset library, including video clips, audio tracks, images, animations, effects, transitions, annotations, cursors, and themes.
layout: schema
name: Camtasia Asset
properties_list:
- description: Unique identifier for the asset
  name: id
  type: string
- description: Display name of the asset
  name: name
  type: string
- description: Description of the asset
  name: description
  type: string
- description: Type of media asset
  name: type
  type: string
- description: File format (e.g., mp4, mp3, png, gif)
  name: format
  type: string
- description: File size in bytes
  name: fileSize
  type: integer
- description: Duration in seconds (for video and audio assets)
  name: duration
  type: number
- description: Width in pixels (for visual assets)
  name: width
  type: integer
- description: Height in pixels (for visual assets)
  name: height
  type: integer
- description: URL to the asset thumbnail image
  name: thumbnailUrl
  type: string
- description: URL to download the asset file
  name: downloadUrl
  type: string
- description: Tags associated with the asset
  name: tags
  type: array
- description: ID of the library containing the asset
  name: libraryId
  type: string
- description: ID of the category this asset belongs to
  name: categoryId
  type: string
- description: When the asset was created
  name: createdAt
  type: string
- description: When the asset was last modified
  name: updatedAt
  type: string
provider_name: Camtasia
provider_slug: camtasia
schema_file: json-schema/camtasia-asset-schema.json
slug: camtasia-asset
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.techsmith.com/schemas/camtasia/asset.json\",\n  \"title\": \"Camtasia Asset\",\n  \"description\": \"Represents a media asset in the Camtasia asset library, including video clips, audio tracks, images, animations, effects, transitions, annotations, cursors, and themes.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the asset\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the asset\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the asset\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"video\",\n        \"audio\",\n        \"image\",\n        \"animation\",\n        \"effect\",\n        \"transition\",\n        \"annotation\",\n        \"cursor\",\n\
  \        \"theme\"\n      ],\n      \"description\": \"Type of media asset\"\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"File format (e.g., mp4, mp3, png, gif)\"\n    },\n    \"fileSize\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"File size in bytes\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"minimum\": 0,\n      \"description\": \"Duration in seconds (for video and audio assets)\"\n    },\n    \"width\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Width in pixels (for visual assets)\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"minimum\": 0,\n      \"description\": \"Height in pixels (for visual assets)\"\n    },\n    \"thumbnailUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to the asset thumbnail image\"\n    },\n    \"downloadUrl\": {\n      \"type\": \"string\",\n      \"format\"\
  : \"uri\",\n      \"description\": \"URL to download the asset file\"\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags associated with the asset\"\n    },\n    \"libraryId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the library containing the asset\"\n    },\n    \"categoryId\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the category this asset belongs to\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the asset was created\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"When the asset was last modified\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"type\"\n  ]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/camtasia/refs/heads/main/json-schema/camtasia-asset-schema.json
tags:
- Screen Recording
- Video Editing
- Tutorial Creation
- E-Learning
- Screencast
- oEmbed
- SDK
title: Camtasia Asset
---
