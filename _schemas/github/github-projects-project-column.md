---
description: Project columns contain cards of work.
layout: schema
name: project-column
properties_list:
- description: ''
  name: url
  type: string
- description: ''
  name: project_url
  type: string
- description: ''
  name: cards_url
  type: string
- description: The unique identifier of the project column
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: Name of the project column
  name: name
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-projects-project-column-schema.json
slug: github-projects-project-column
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-project-column-schema.json\",\n  \"title\": \"project-column\",\n  \"description\": \"Project columns contain cards of work.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/projects/columns/367\"\n    },\n    \"project_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/projects/120\"\n    },\n    \"cards_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/projects/columns/367/cards\"\n    },\n    \"id\": {\n      \"description\": \"The unique identifier of the project column\",\n      \"example\": 42,\n      \"type\": \"integer\"\n    },\n    \"node_id\": {\n  \
  \    \"type\": \"string\",\n      \"example\": \"MDEzOlByb2plY3RDb2x1bW4zNjc=\"\n    },\n    \"name\": {\n      \"description\": \"Name of the project column\",\n      \"example\": \"Remaining tasks\",\n      \"type\": \"string\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-09-05T14:18:44Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-09-05T14:22:28Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"url\",\n    \"project_url\",\n    \"cards_url\",\n    \"name\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-project-column-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: project-column
---
