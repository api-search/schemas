---
description: Project cards represent a scope of work.
layout: schema
name: project-card
properties_list:
- description: ''
  name: url
  type: string
- description: The project card's ID
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: ''
  name: note
  type: string
- description: ''
  name: creator
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: Whether or not the card is archived
  name: archived
  type: boolean
- description: ''
  name: column_name
  type: string
- description: ''
  name: project_id
  type: string
- description: ''
  name: column_url
  type: string
- description: ''
  name: content_url
  type: string
- description: ''
  name: project_url
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-projects-project-card-schema.json
slug: github-projects-project-card
source_filename: github-projects-project-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-project-card-schema.json\",\n  \"title\": \"project-card\",\n  \"description\": \"Project cards represent a scope of work.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/projects/columns/cards/1478\"\n    },\n    \"id\": {\n      \"description\": \"The project card's ID\",\n      \"example\": 42,\n      \"type\": \"integer\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDExOlByb2plY3RDYXJkMTQ3OA==\"\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"example\": \"Add payload for delete Project column\",\n      \"nullable\": true\n    },\n    \"creator\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"\
  created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-09-05T14:21:06Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2016-09-05T14:20:22Z\"\n    },\n    \"archived\": {\n      \"description\": \"Whether or not the card is archived\",\n      \"example\": false,\n      \"type\": \"boolean\"\n    },\n    \"column_name\": {\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"project_id\": {\n      \"type\": \"string\",\n      \"example\": \"12345678\"\n    },\n    \"column_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/projects/columns/367\"\n    },\n    \"content_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/api-playground/projects-test/issues/3\"\n    },\n    \"project_url\": {\n      \"type\": \"string\",\n  \
  \    \"format\": \"uri\",\n      \"example\": \"https://api.github.com/projects/120\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"note\",\n    \"url\",\n    \"column_url\",\n    \"project_url\",\n    \"creator\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-project-card-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: project-card
---
