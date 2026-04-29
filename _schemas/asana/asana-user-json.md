---
description: A user object represents an account in Asana that can be given access to various workspaces, projects, and tasks. The special string identifier 'me' can be used to refer to the current authenticated user.
layout: schema
name: Asana User
properties_list:
- description: Globally unique identifier of the resource.
  name: gid
  type: string
- description: The base type of this resource.
  name: resource_type
  type: string
- description: The user's name. Read-only except when same user as requester.
  name: name
  type: string
- description: The user's email address.
  name: email
  type: string
- description: A map of the user's profile photo in various sizes.
  name: photo
  type:
  - object
  - 'null'
- description: Workspaces and organizations this user may access.
  name: workspaces
  type: array
provider_name: Asana
provider_slug: asana
schema_file: json-schema/asana-user-json-schema.json
slug: asana-user-json
source_filename: asana-user-json-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://developers.asana.com/schemas/user\",\n  \"title\": \"Asana User\",\n  \"description\": \"A user object represents an account in Asana that can be given access to various workspaces, projects, and tasks. The special string identifier 'me' can be used to refer to the current authenticated user.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gid\": {\n      \"type\": \"string\",\n      \"description\": \"Globally unique identifier of the resource.\",\n      \"readOnly\": true,\n      \"examples\": [\"12345\"]\n    },\n    \"resource_type\": {\n      \"type\": \"string\",\n      \"const\": \"user\",\n      \"description\": \"The base type of this resource.\",\n      \"readOnly\": true\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The user's name. Read-only except when same user as requester.\",\n      \"examples\": [\"Greg Sanchez\"]\n    },\n   \
  \ \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The user's email address.\",\n      \"readOnly\": true,\n      \"examples\": [\"gsanchez@example.com\"]\n    },\n    \"photo\": {\n      \"type\": [\"object\", \"null\"],\n      \"description\": \"A map of the user's profile photo in various sizes.\",\n      \"readOnly\": true,\n      \"properties\": {\n        \"image_21x21\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"image_27x27\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"image_36x36\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"image_60x60\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"image_128x128\": { \"type\": \"string\", \"format\": \"uri\" },\n        \"image_1024x1024\": { \"type\": \"string\", \"format\": \"uri\" }\n      }\n    },\n    \"workspaces\": {\n      \"type\": \"array\",\n      \"items\": { \"$ref\": \"#/$defs/WorkspaceCompact\" },\n      \"description\"\
  : \"Workspaces and organizations this user may access.\",\n      \"readOnly\": true\n    }\n  },\n  \"required\": [\"gid\", \"resource_type\"],\n  \"$defs\": {\n    \"WorkspaceCompact\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gid\": { \"type\": \"string\" },\n        \"resource_type\": { \"type\": \"string\", \"const\": \"workspace\" },\n        \"name\": { \"type\": \"string\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/asana/refs/heads/main/json-schema/asana-user-json-schema.json
tags:
- Collaboration
- Productivity
- Project Management
- Projects
- Task Management
- Tasks
- Workflow
title: Asana User
---
