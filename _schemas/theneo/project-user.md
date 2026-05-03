---
description: A Project User represents a user who has been granted access to a specific API documentation project on the Theneo platform, with a designated role.
layout: schema
name: Theneo Project User
properties_list:
- description: The unique identifier of the user.
  name: id
  type: string
- description: The email address of the user.
  name: email
  type: string
- description: The access role of the user on the project.
  name: role
  type: string
- description: The name of the user.
  name: name
  type: string
provider_name: Theneo
provider_slug: theneo
schema_file: json-schema/project-user.json
slug: project-user
source_filename: project-user.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/theneo/blob/main/json-schema/project-user.json\",\n  \"title\": \"Theneo Project User\",\n  \"description\": \"A Project User represents a user who has been granted access to a specific API documentation project on the Theneo platform, with a designated role.\",\n  \"type\": \"object\",\n  \"required\": [\"email\", \"role\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the user.\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"format\": \"email\",\n      \"description\": \"The email address of the user.\"\n    },\n    \"role\": {\n      \"type\": \"string\",\n      \"enum\": [\"viewer\", \"editor\", \"admin\"],\n      \"description\": \"The access role of the user on the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of\
  \ the user.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/json-schema/project-user.json
tags:
- Change Logs
- Documentation
- Platform
title: Theneo Project User
---
