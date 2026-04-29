---
description: Starred Repository
layout: schema
name: starred-repository
properties_list:
- description: ''
  name: starred_at
  type: string
- description: ''
  name: repo
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-users-api-starred-repository-schema.json
slug: github-users-api-starred-repository
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-users-api-starred-repository-schema.json\",\n  \"title\": \"starred-repository\",\n  \"description\": \"Starred Repository\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"starred_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"repo\": {\n      \"$ref\": \"#/components/schemas/repository\"\n    }\n  },\n  \"required\": [\n    \"starred_at\",\n    \"repo\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-users-api-starred-repository-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: starred-repository
---
