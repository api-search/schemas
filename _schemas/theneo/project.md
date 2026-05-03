---
description: A Project represents an API documentation project on the Theneo platform, containing imported API specifications and published documentation.
layout: schema
name: Theneo Project
properties_list:
- description: The unique identifier of the project.
  name: id
  type: string
- description: The name of the project.
  name: name
  type: string
- description: The URL-friendly slug of the project.
  name: slug
  type: string
- description: The identifier of the workspace this project belongs to.
  name: workspaceId
  type: string
- description: A description of the project.
  name: description
  type: string
- description: Whether the project documentation is published.
  name: published
  type: boolean
- description: The timestamp when the project was created.
  name: createdAt
  type: string
- description: The timestamp when the project was last updated.
  name: updatedAt
  type: string
provider_name: Theneo
provider_slug: theneo
schema_file: json-schema/project.json
slug: project
source_filename: project.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/theneo/blob/main/json-schema/project.json\",\n  \"title\": \"Theneo Project\",\n  \"description\": \"A Project represents an API documentation project on the Theneo platform, containing imported API specifications and published documentation.\",\n  \"type\": \"object\",\n  \"required\": [\"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the project.\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The URL-friendly slug of the project.\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"The identifier of the workspace this project belongs to.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"A description of the project.\"\n    },\n    \"published\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the project documentation is published.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the project was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The timestamp when the project was last updated.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/theneo/refs/heads/main/json-schema/project.json
tags:
- Change Logs
- Documentation
- Platform
title: Theneo Project
---
