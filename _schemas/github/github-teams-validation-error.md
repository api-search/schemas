---
description: Validation Error
layout: schema
name: validation-error
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
schema_file: json-schema/github-teams-validation-error-schema.json
slug: github-teams-validation-error
source_filename: github-teams-validation-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-validation-error-schema.json\",\n  \"title\": \"validation-error\",\n  \"description\": \"Validation Error\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"Example body text\"\n    },\n    \"documentation_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"required\": [\n          \"code\"\n        ],\n        \"properties\": {\n          \"resource\": {\n            \"type\": \"string\"\n          },\n          \"field\": {\n            \"type\": \"string\"\n          },\n          \"message\": {\n            \"type\": \"string\"\n          },\n         \
  \ \"code\": {\n            \"type\": \"string\"\n          },\n          \"index\": {\n            \"type\": \"integer\"\n          },\n          \"value\": {\n            \"oneOf\": [\n              {\n                \"type\": \"string\",\n                \"nullable\": true\n              },\n              {\n                \"type\": \"integer\",\n                \"nullable\": true\n              },\n              {\n                \"type\": \"array\",\n                \"nullable\": true,\n                \"items\": {\n                  \"type\": \"string\"\n                }\n              }\n            ]\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"message\",\n    \"documentation_url\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-teams-validation-error-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: validation-error
---
