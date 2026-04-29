---
description: Base Gist
layout: schema
name: base-gist
properties_list:
- description: ''
  name: url
  type: string
- description: ''
  name: forks_url
  type: string
- description: ''
  name: commits_url
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: node_id
  type: string
- description: ''
  name: git_pull_url
  type: string
- description: ''
  name: git_push_url
  type: string
- description: ''
  name: html_url
  type: string
- description: ''
  name: files
  type: object
- description: ''
  name: public
  type: boolean
- description: ''
  name: created_at
  type: string
- description: ''
  name: updated_at
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: comments
  type: integer
- description: ''
  name: user
  type: object
- description: ''
  name: comments_url
  type: string
- description: ''
  name: owner
  type: object
- description: ''
  name: truncated
  type: boolean
- description: ''
  name: forks
  type: array
- description: ''
  name: history
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-gists-base-gist-schema.json
slug: github-gists-base-gist
source_filename: github-gists-base-gist-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-gists-base-gist-schema.json\",\n  \"title\": \"base-gist\",\n  \"description\": \"Base Gist\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"forks_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"commits_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"12345678\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"12345678\"\n    },\n    \"git_pull_url\":\
  \ {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"git_push_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"files\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"filename\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\"\n          },\n          \"language\": {\n            \"type\": \"string\"\n          },\n          \"raw_url\": {\n            \"type\": \"string\"\n          },\n          \"size\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n\
  \    \"public\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"updated_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2026-04-17T12:00:00Z\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"nullable\": true,\n      \"example\": \"This is an example repository\"\n    },\n    \"comments\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"comments_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/simple-user\"\n    },\n    \"truncated\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n\
  \    \"forks\": {\n      \"type\": \"array\",\n      \"items\": {}\n    },\n    \"history\": {\n      \"type\": \"array\",\n      \"items\": {}\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"node_id\",\n    \"url\",\n    \"forks_url\",\n    \"commits_url\",\n    \"git_pull_url\",\n    \"git_push_url\",\n    \"html_url\",\n    \"comments_url\",\n    \"public\",\n    \"description\",\n    \"comments\",\n    \"user\",\n    \"files\",\n    \"created_at\",\n    \"updated_at\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-gists-base-gist-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: base-gist
---
