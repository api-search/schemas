---
description: Basic Error
layout: schema
name: basic-error
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: documentation_url
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: status
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-collaborators-api-basic-error-schema.json
slug: github-repo-collaborators-api-basic-error
source_filename: github-repo-collaborators-api-basic-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-collaborators-api-basic-error-schema.json\",\n  \"title\": \"basic-error\",\n  \"description\": \"Basic Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Example body text\"\n    },\n    \"documentation_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"open\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-collaborators-api-basic-error-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: basic-error
---
