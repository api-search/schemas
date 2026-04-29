---
description: The authorization for an OAuth app, GitHub App, or a Personal Access Token.
layout: schema
name: authorization
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: url
  type: string
- description: A list of scopes that this authorization is in.
  name: scopes
  type: array
- description: ''
  name: token
  type: string
- description: ''
  name: token_last_eight
  type: string
- description: ''
  name: hashed_token
  type: string
- description: ''
  name: app
  type: object
- description: ''
  name: note
  type: string
- description: ''
  name: note_url
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: fingerprint
  type: string
- description: ''
  name: user
  type: object
- description: ''
  name: installation
  type: object
- description: ''
  name: expires_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-app-api-authorization-schema.json
slug: github-app-api-authorization
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-app-api-authorization-schema.json\",\n  \"title\": \"authorization\",\n  \"description\": \"The authorization for an OAuth app, GitHub App, or a Personal Access Token.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"scopes\": {\n      \"description\": \"A list of scopes that this authorization is in.\",\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"nullable\": true\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"token_last_eight\": {\n      \"type\": \"string\"\
  ,\n      \"nullable\": true,\n      \"example\": \"example_value\"\n    },\n    \"hashed_token\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"example_value\"\n    },\n    \"app\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"client_id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\n        \"client_id\",\n        \"name\",\n        \"url\"\n      ]\n    },\n    \"note\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"example_value\"\n    },\n    \"note_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"nullable\": true,\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\
  ,\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"fingerprint\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"example_value\"\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"installation\": {\n      \"$ref\": \"#/components/schemas/nullable-scoped-installation\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"nullable\": true,\n      \"example\": \"2026-04-17T12:00:00Z\"\n    }\n  },\n  \"required\": [\n    \"app\",\n    \"id\",\n    \"note\",\n    \"note_url\",\n    \"scopes\",\n    \"token\",\n    \"hashed_token\",\n    \"token_last_eight\",\n    \"fingerprint\",\n    \"url\",\n    \"created_at\",\n    \"updated_at\",\n    \"expires_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-app-api-authorization-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: authorization
---
