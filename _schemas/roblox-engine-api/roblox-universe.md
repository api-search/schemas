---
description: Schema for a Roblox experience (universe) resource from the Open Cloud API.
layout: schema
name: Roblox Universe
properties_list:
- description: Unique universe identifier
  name: id
  type: string
- description: Public display name of the experience
  name: displayName
  type: string
- description: Description of the experience
  name: description
  type: string
- description: Whether the experience is publicly visible
  name: visibility
  type: string
- description: Associated social media links
  name: socialLinks
  type: array
- description: Timestamp when the universe was created
  name: createTime
  type: string
- description: Timestamp of the last update
  name: updateTime
  type: string
provider_name: Roblox Engine API
provider_slug: roblox-engine-api
schema_file: json-schema/roblox-universe-schema.json
slug: roblox-universe
source_filename: roblox-universe-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/roblox-engine-api/json-schema/roblox-universe-schema.json\",\n  \"title\": \"Roblox Universe\",\n  \"description\": \"Schema for a Roblox experience (universe) resource from the Open Cloud API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique universe identifier\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Public display name of the experience\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the experience\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"public\", \"private\"],\n      \"description\": \"Whether the experience is publicly visible\"\n    },\n    \"socialLinks\": {\n      \"type\": \"array\",\n      \"description\": \"Associated social media links\"\
  ,\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": { \"type\": \"string\" },\n          \"url\": { \"type\": \"string\", \"format\": \"uri\" }\n        }\n      }\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the universe was created\"\n    },\n    \"updateTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp of the last update\"\n    }\n  },\n  \"required\": [\"id\", \"displayName\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/json-schema/roblox-universe-schema.json
tags:
- Gaming
- Game Development
- Metaverse
- Roblox
- Open Cloud
title: Roblox Universe
---
