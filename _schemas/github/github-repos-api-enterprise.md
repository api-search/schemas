---
description: An enterprise on GitHub.
layout: schema
name: enterprise
properties_list:
- description: short description of the enterprise.
  name: description
  type: string
- description: ''
  name: html_url
  type: string
- description: The enterprise's website URL.
  name: website_url
  type: string
- description: Unique identifier of the enterprise
  name: id
  type: integer
- description: ''
  name: node_id
  type: string
- description: The name of the enterprise.
  name: name
  type: string
- description: The slug url identifier for the enterprise.
  name: slug
  type: string
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: avatar_url
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repos-api-enterprise-schema.json
slug: github-repos-api-enterprise
source_filename: github-repos-api-enterprise-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repos-api-enterprise-schema.json\",\n  \"title\": \"enterprise\",\n  \"description\": \"An enterprise on GitHub.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"description\": {\n      \"description\": \"short description of the enterprise.\",\n      \"type\": \"string\",\n      \"example\": \"This is an example repository\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://github.com/enterprises/octo-business\"\n    },\n    \"website_url\": {\n      \"description\": \"The enterprise's website URL.\",\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"id\": {\n      \"description\": \"Unique identifier of the enterprise\",\n      \"example\"\
  : 42,\n      \"type\": \"integer\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDEwOlJlcG9zaXRvcnkxMjk2MjY5\"\n    },\n    \"name\": {\n      \"description\": \"The name of the enterprise.\",\n      \"type\": \"string\",\n      \"example\": \"Octo Business\"\n    },\n    \"slug\": {\n      \"description\": \"The slug url identifier for the enterprise.\",\n      \"type\": \"string\",\n      \"example\": \"octo-business\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2019-01-26T19:01:12Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2019-01-26T19:14:43Z\"\n    },\n    \"avatar_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"name\",\n    \"slug\",\n    \"html_url\"\
  ,\n    \"created_at\",\n    \"updated_at\",\n    \"avatar_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repos-api-enterprise-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: enterprise
---
