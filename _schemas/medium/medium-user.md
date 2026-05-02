---
description: A Medium user profile containing identifying information, username, display name, profile URL, and avatar image.
layout: schema
name: Medium User
properties_list:
- description: The unique identifier for the user on Medium.
  name: id
  type: string
- description: The user's username on Medium, used in their profile URL path.
  name: username
  type: string
- description: The user's display name as shown on their profile.
  name: name
  type: string
- description: The URL to the user's Medium profile page.
  name: url
  type: string
- description: The URL to the user's avatar image on Medium.
  name: imageUrl
  type: string
provider_name: medium
provider_slug: medium
schema_file: json-schema/medium-user-schema.json
slug: medium-user
source_filename: medium-user-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://medium.com/schemas/medium/user.json\",\n  \"title\": \"Medium User\",\n  \"description\": \"A Medium user profile containing identifying information, username, display name, profile URL, and avatar image.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"username\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the user on Medium.\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"The user's username on Medium, used in their profile URL path.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The user's display name as shown on their profile.\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the user's Medium profile page.\"\n    },\n    \"imageUrl\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to the user's avatar image on Medium.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/medium/refs/heads/main/json-schema/medium-user-schema.json
tags: []
title: Medium User
---
