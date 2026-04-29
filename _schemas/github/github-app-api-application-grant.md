---
description: The authorization associated with an OAuth Access.
layout: schema
name: application-grant
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: url
  type: string
- description: ''
  name: app
  type: object
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: scopes
  type: array
- description: ''
  name: user
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-app-api-application-grant-schema.json
slug: github-app-api-application-grant
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-app-api-application-grant-schema.json\",\n  \"title\": \"application-grant\",\n  \"description\": \"The authorization associated with an OAuth Access.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/applications/grants/1\"\n    },\n    \"app\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"client_id\": {\n          \"type\": \"string\"\n        },\n        \"name\": {\n          \"type\": \"string\"\n        },\n        \"url\": {\n          \"type\": \"string\",\n          \"format\": \"uri\"\n        }\n      },\n      \"required\": [\n        \"client_id\",\n        \"name\",\n        \"url\"\
  \n      ]\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-09-06T17:26:27Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2011-09-06T20:39:23Z\"\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"public_repo\"\n      ]\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    }\n  },\n  \"required\": [\n    \"app\",\n    \"id\",\n    \"scopes\",\n    \"url\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-app-api-application-grant-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: application-grant
---
