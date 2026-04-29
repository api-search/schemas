---
description: Project Collaborator Permission
layout: schema
name: project-collaborator-permission
properties_list:
- description: ''
  name: permission
  type: string
- description: ''
  name: user
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-projects-project-collaborator-permission-schema.json
slug: github-projects-project-collaborator-permission
source_filename: github-projects-project-collaborator-permission-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-project-collaborator-permission-schema.json\",\n  \"title\": \"project-collaborator-permission\",\n  \"description\": \"Project Collaborator Permission\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permission\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    }\n  },\n  \"required\": [\n    \"permission\",\n    \"user\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-projects-project-collaborator-permission-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: project-collaborator-permission
---
