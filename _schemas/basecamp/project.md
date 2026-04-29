---
description: ''
layout: schema
name: Project
properties_list:
- description: Unique project identifier
  name: id
  type: integer
- description: Project status (active, archived, trashed)
  name: status
  type: string
- description: Timestamp when the project was created
  name: created_at
  type: string
- description: Timestamp when the project was last updated
  name: updated_at
  type: string
- description: Project name
  name: name
  type: string
- description: Project description
  name: description
  type: string
- description: Project purpose classification
  name: purpose
  type: string
- description: Whether client access is enabled for this project
  name: clients_enabled
  type: boolean
- description: Whether timesheets are enabled for this project
  name: timesheet_enabled
  type: boolean
- description: Project color identifier
  name: color
  type: string
- description: API URL for this project
  name: url
  type: string
- description: Web URL for this project
  name: app_url
  type: string
- description: API URL to bookmark this project
  name: bookmark_url
  type: string
- description: List of tools available on this project
  name: dock
  type: array
provider_name: Basecamp
provider_slug: basecamp
schema_file: json-schema/project-schema.json
slug: project
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/basecamp/json-schema/project-schema.json\",\n  \"title\": \"Project\",\n  \"type\": \"object\",\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"status\"\n  ],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Unique project identifier\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Project status (active, archived, trashed)\",\n      \"enum\": [\n        \"active\",\n        \"archived\",\n        \"trashed\"\n      ]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was created\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the project was last updated\"\n    },\n    \"name\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Project name\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Project description\",\n      \"nullable\": true\n    },\n    \"purpose\": {\n      \"type\": \"string\",\n      \"description\": \"Project purpose classification\"\n    },\n    \"clients_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether client access is enabled for this project\"\n    },\n    \"timesheet_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether timesheets are enabled for this project\"\n    },\n    \"color\": {\n      \"type\": \"string\",\n      \"description\": \"Project color identifier\",\n      \"nullable\": true\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL for this project\"\n    },\n    \"app_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Web URL for this project\"\
  \n    },\n    \"bookmark_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"API URL to bookmark this project\"\n    },\n    \"dock\": {\n      \"type\": \"array\",\n      \"description\": \"List of tools available on this project\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/DockItem\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/json-schema/project-schema.json
tags:
- Collaboration
- Project Management
- REST
- SaaS
- Team Communication
title: Project
---
