---
description: Validation Error Simple
layout: schema
name: validation-error-simple
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: documentation_url
  type: string
- description: ''
  name: errors
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repos-api-validation-error-simple-schema.json
slug: github-repos-api-validation-error-simple
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repos-api-validation-error-simple-schema.json\",\n  \"title\": \"validation-error-simple\",\n  \"description\": \"Validation Error Simple\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Example body text\"\n    },\n    \"documentation_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"message\",\n    \"documentation_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repos-api-validation-error-simple-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: validation-error-simple
---
