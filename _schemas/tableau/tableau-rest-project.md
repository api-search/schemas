---
description: ''
layout: schema
name: Project
properties_list:
- description: The unique identifier for the project.
  name: id
  type: string
- description: The name of the project.
  name: name
  type: string
- description: A description of the project.
  name: description
  type: string
- description: The ID of the parent project. If null, this is a top-level project.
  name: parentProjectId
  type: '[''string'', ''null'']'
- description: The permissions model for the project.
  name: contentPermissions
  type: string
- description: The date and time the project was created.
  name: createdAt
  type: string
- description: The date and time the project was last updated.
  name: updatedAt
  type: string
- description: ''
  name: owner
  type: object
- description: Whether this is a top-level project.
  name: topLevelProject
  type: boolean
provider_name: Tableau
provider_slug: tableau
schema_file: json-schema/tableau-rest-project-schema.json
slug: tableau-rest-project
source_filename: tableau-rest-project-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Project\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the project.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the project.\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description of the project.\"\n    },\n    \"parentProjectId\": {\n      \"type\": \"['string', 'null']\",\n      \"description\": \"The ID of the parent project. If null, this is a top-level project.\"\n    },\n    \"contentPermissions\": {\n      \"type\": \"string\",\n      \"description\": \"The permissions model for the project.\"\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"description\": \"The date and time the project was created.\"\n    },\n    \"updatedAt\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The date and time the project was last updated.\"\n    },\n    \"owner\": {\n      \"type\": \"object\"\n    },\n    \"topLevelProject\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a top-level project.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tableau/refs/heads/main/json-schema/tableau-rest-project-schema.json
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
title: Project
---
