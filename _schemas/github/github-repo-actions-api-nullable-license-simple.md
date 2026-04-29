---
description: License Simple
layout: schema
name: nullable-license-simple
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: spdx_id
  type: string
- description: ''
  name: node_id
  type: string
- description: ''
  name: html_url
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-actions-api-nullable-license-simple-schema.json
slug: github-repo-actions-api-nullable-license-simple
source_filename: github-repo-actions-api-nullable-license-simple-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-actions-api-nullable-license-simple-schema.json\",\n  \"title\": \"nullable-license-simple\",\n  \"description\": \"License Simple\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"mit\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"MIT License\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/licenses/mit\"\n    },\n    \"spdx_id\": {\n      \"type\": \"string\",\n      \"example\": \"MIT\"\n    },\n    \"node_id\": {\n      \"type\": \"string\",\n      \"example\": \"MDc6TGljZW5zZW1pdA==\"\n    },\n    \"html_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"example\": \"https://api.github.com/repos/octocat/Hello-World\"\
  \n    }\n  },\n  \"required\": [\n    \"key\",\n    \"name\",\n    \"url\",\n    \"spdx_id\",\n    \"node_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-actions-api-nullable-license-simple-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: nullable-license-simple
---
