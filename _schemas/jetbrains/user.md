---
description: A user resource common across JetBrains Hub, YouTrack, TeamCity, and Space.
layout: schema
name: JetBrains User
properties_list:
- description: Unique identifier for the user.
  name: id
  type: string
- description: Login name of the user.
  name: login
  type: string
- description: Full display name of the user.
  name: fullName
  type: string
- description: Email address of the user.
  name: email
  type: string
- description: URL of the user avatar image.
  name: avatarUrl
  type: string
- description: Whether the user account is banned.
  name: banned
  type: boolean
- description: Groups the user belongs to.
  name: groups
  type: array
provider_name: JetBrains
provider_slug: jetbrains
schema_file: json-schema/user.json
slug: user
source_filename: user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jetbrains-user.json\",\n  \"title\": \"JetBrains User\",\n  \"description\": \"A user resource common across JetBrains Hub, YouTrack, TeamCity, and Space.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the user.\"\n    },\n    \"login\": {\n      \"type\": \"string\",\n      \"description\": \"Login name of the user.\"\n    },\n    \"fullName\": {\n      \"type\": \"string\",\n      \"description\": \"Full display name of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"Email address of the user.\"\n    },\n    \"avatarUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the user avatar image.\"\n    },\n    \"banned\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the user account is banned.\"\n    },\n    \"groups\": {\n      \"type\": \"array\",\n      \"description\": \"Groups the user belongs to.\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": { \"type\": \"string\" },\n          \"name\": { \"type\": \"string\" }\n        }\n      }\n    }\n  },\n  \"required\": [\"id\", \"login\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/json-schema/user.json
tags:
- CI/CD
- Developer Tools
- IDE
title: JetBrains User
---
