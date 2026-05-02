---
description: A project resource common across JetBrains products including Space, TeamCity, and YouTrack.
layout: schema
name: JetBrains Project
properties_list:
- description: Unique identifier for the project.
  name: id
  type: string
- description: Human-readable name of the project.
  name: name
  type: string
- description: Short key or abbreviation for the project.
  name: key
  type: string
- description: Description of the project.
  name: description
  type: string
- description: Whether the project is archived.
  name: archived
  type: boolean
- description: Timestamp when the project was created.
  name: createdAt
  type: string
provider_name: JetBrains
provider_slug: jetbrains
schema_file: json-schema/project.json
slug: project
source_filename: project.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"jetbrains-project.json\",\n  \"title\": \"JetBrains Project\",\n  \"description\": \"A project resource common across JetBrains products including Space, TeamCity, and YouTrack.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable name of the project.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"Short key or abbreviation for the project.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the project.\"\n    },\n    \"archived\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project is archived.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n\
  \      \"description\": \"Timestamp when the project was created.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/jetbrains/refs/heads/main/json-schema/project.json
tags:
- CI/CD
- Developer Tools
- IDE
title: JetBrains Project
---
