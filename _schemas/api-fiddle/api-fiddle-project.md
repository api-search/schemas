---
description: An API design project within the API Fiddle platform containing one or more API specifications.
layout: schema
name: API Fiddle Project
properties_list:
- description: Unique identifier for the project.
  name: id
  type: string
- description: Name of the project.
  name: name
  type: string
- description: A detailed description of the project.
  name: description
  type: string
- description: Identifier of the workspace this project belongs to.
  name: workspaceId
  type: string
- description: Visibility level of the project.
  name: visibility
  type: string
- description: List of specifications associated with this project.
  name: specifications
  type: array
- description: Tags for categorizing the project.
  name: tags
  type: array
- description: Timestamp when the project was created.
  name: createdAt
  type: string
- description: Timestamp when the project was last updated.
  name: updatedAt
  type: string
provider_name: API-Fiddle
provider_slug: api-fiddle
schema_file: json-schema/api-fiddle-project-schema.json
slug: api-fiddle-project
source_filename: api-fiddle-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-fiddle.com/schemas/project.json\",\n  \"title\": \"API Fiddle Project\",\n  \"description\": \"An API design project within the API Fiddle platform containing one or more API specifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the project.\",\n      \"minLength\": 1,\n      \"maxLength\": 255\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A detailed description of the project.\"\n    },\n    \"workspaceId\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the workspace this project belongs to.\"\n    },\n    \"visibility\": {\n      \"type\": \"string\",\n      \"enum\": [\"private\", \"public\", \"shared\"],\n    \
  \  \"description\": \"Visibility level of the project.\",\n      \"default\": \"private\"\n    },\n    \"specifications\": {\n      \"type\": \"array\",\n      \"description\": \"List of specifications associated with this project.\",\n      \"items\": {\n        \"$ref\": \"api-fiddle-specification-schema.json\"\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"description\": \"Tags for categorizing the project.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was last updated.\"\n    }\n  },\n  \"required\": [\"id\", \"name\"],\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/api-fiddle/refs/heads/main/json-schema/api-fiddle-project-schema.json
tags:
- API Design
- OpenAPI
- Collaboration
- Documentation
- Platform
title: API Fiddle Project
---
