---
description: Gist Commit
layout: schema
name: gist-commit
properties_list:
- description: ''
  name: url
  type: string
- description: ''
  name: version
  type: string
- description: ''
  name: user
  type: object
- description: ''
  name: change_status
  type: object
- description: ''
  name: committed_at
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-gists-gist-commit-schema.json
slug: github-gists-gist-commit
source_filename: github-gists-gist-commit-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-gists-gist-commit-schema.json\",\n  \"title\": \"gist-commit\",\n  \"description\": \"Gist Commit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/gists/aa5a315d61ae9438b18d/57a7f021a713b1c5a6a199b54cc514735d2d462f\"\n    },\n    \"version\": {\n      \"type\": \"string\",\n      \"example\": \"57a7f021a713b1c5a6a199b54cc514735d2d462f\"\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/nullable-simple-user\"\n    },\n    \"change_status\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"total\": {\n          \"type\": \"integer\"\n        },\n        \"additions\": {\n          \"type\": \"integer\"\n        },\n        \"deletions\": {\n          \"type\"\
  : \"integer\"\n        }\n      }\n    },\n    \"committed_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"2010-04-14T02:15:15Z\"\n    }\n  },\n  \"required\": [\n    \"url\",\n    \"user\",\n    \"version\",\n    \"committed_at\",\n    \"change_status\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-gists-gist-commit-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: gist-commit
---
