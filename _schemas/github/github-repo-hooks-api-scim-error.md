---
description: Scim Error
layout: schema
name: scim-error
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: documentation_url
  type: string
- description: ''
  name: detail
  type: string
- description: ''
  name: status
  type: integer
- description: ''
  name: scimType
  type: string
- description: ''
  name: schemas
  type: array
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-hooks-api-scim-error-schema.json
slug: github-repo-hooks-api-scim-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-hooks-api-scim-error-schema.json\",\n  \"title\": \"scim-error\",\n  \"description\": \"Scim Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Example body text\"\n    },\n    \"documentation_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"detail\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"status\": {\n      \"type\": \"integer\",\n      \"example\": 42\n    },\n    \"scimType\": {\n      \"type\": \"string\",\n      \"example\": \"User\"\n    },\n    \"schemas\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-hooks-api-scim-error-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: scim-error
---
