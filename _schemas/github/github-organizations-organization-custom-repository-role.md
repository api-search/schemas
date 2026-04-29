---
description: Custom repository roles created by organization owners
layout: schema
name: organization-custom-repository-role
properties_list:
- description: The unique identifier of the custom role.
  name: id
  type: integer
- description: The name of the custom role.
  name: name
  type: string
- description: A short description about who this role is for or what permissions it grants.
  name: description
  type: string
- description: The system role from which this role inherits permissions.
  name: base_role
  type: string
- description: A list of additional permissions included in this role.
  name: permissions
  type: array
- description: ''
  name: organization
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-organizations-organization-custom-repository-role-schema.json
slug: github-organizations-organization-custom-repository-role
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organizations-organization-custom-repository-role-schema.json\",\n  \"title\": \"organization-custom-repository-role\",\n  \"description\": \"Custom repository roles created by organization owners\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"description\": \"The unique identifier of the custom role.\",\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"name\": {\n      \"description\": \"The name of the custom role.\",\n      \"type\": \"string\",\n      \"example\": \"octocat\"\n    },\n    \"description\": {\n      \"description\": \"A short description about who this role is for or what permissions it grants.\",\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"This is an example repository\"\n    },\n    \"base_role\": {\n     \
  \ \"type\": \"string\",\n      \"description\": \"The system role from which this role inherits permissions.\",\n      \"enum\": [\n        \"read\",\n        \"triage\",\n        \"write\",\n        \"maintain\"\n      ],\n      \"example\": \"read\"\n    },\n    \"permissions\": {\n      \"description\": \"A list of additional permissions included in this role.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"organization\": {\n      \"$ref\": \"#/components/schemas/simple-user\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"name\",\n    \"base_role\",\n    \"permissions\",\n    \"organization\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-organizations-organization-custom-repository-role-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: organization-custom-repository-role
---
