---
description: Schema for a Roblox user resource from the Open Cloud API.
layout: schema
name: Roblox User
properties_list:
- description: Resource path in format users/{userId}
  name: path
  type: string
- description: Account creation timestamp
  name: createTime
  type: string
- description: Unique Roblox user identifier
  name: id
  type: string
- description: Unique username
  name: name
  type: string
- description: Display name shown in-game
  name: displayName
  type: string
- description: User profile bio
  name: about
  type: string
- description: User locale setting
  name: locale
  type: string
- description: Whether the user has Roblox Premium
  name: premium
  type: boolean
- description: Whether the user's identity has been verified
  name: idVerified
  type: boolean
provider_name: Roblox Engine API
provider_slug: roblox-engine-api
schema_file: json-schema/roblox-user-schema.json
slug: roblox-user
source_filename: roblox-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/roblox-engine-api/json-schema/roblox-user-schema.json\",\n  \"title\": \"Roblox User\",\n  \"description\": \"Schema for a Roblox user resource from the Open Cloud API.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"path\": {\n      \"type\": \"string\",\n      \"description\": \"Resource path in format users/{userId}\"\n    },\n    \"createTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Account creation timestamp\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique Roblox user identifier\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Unique username\"\n    },\n    \"displayName\": {\n      \"type\": \"string\",\n      \"description\": \"Display name shown in-game\"\n    },\n    \"about\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"User profile bio\"\n    },\n    \"locale\": {\n      \"type\": \"string\",\n      \"description\": \"User locale setting\"\n    },\n    \"premium\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user has Roblox Premium\"\n    },\n    \"idVerified\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the user's identity has been verified\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/roblox-engine-api/refs/heads/main/json-schema/roblox-user-schema.json
tags:
- Gaming
- Game Development
- Metaverse
- Roblox
- Open Cloud
title: Roblox User
---
