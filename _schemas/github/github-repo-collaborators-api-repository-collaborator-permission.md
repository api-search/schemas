---
description: Repository Collaborator Permission
layout: schema
name: repository-collaborator-permission
properties_list:
- description: ''
  name: permission
  type: string
- description: ''
  name: role_name
  type: string
- description: ''
  name: user
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-collaborators-api-repository-collaborator-permission-schema.json
slug: github-repo-collaborators-api-repository-collaborator-permission
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-collaborators-api-repository-collaborator-permission-schema.json\",\n  \"title\": \"repository-collaborator-permission\",\n  \"description\": \"Repository Collaborator Permission\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"permission\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"role_name\": {\n      \"type\": \"string\",\n      \"example\": \"admin\"\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/nullable-collaborator\"\n    }\n  },\n  \"required\": [\n    \"permission\",\n    \"role_name\",\n    \"user\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-collaborators-api-repository-collaborator-permission-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: repository-collaborator-permission
---
