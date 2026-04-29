---
description: ''
layout: schema
name: SimpleCommit
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: tree_id
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: timestamp
  type: string
- description: ''
  name: author
  type: object
- description: ''
  name: committer
  type: object
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-simple-commit-schema.json
slug: github-actions-simple-commit
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SimpleCommit\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"tree_id\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"timestamp\": {\n      \"type\": \"string\"\n    },\n    \"author\": {\n      \"type\": \"object\"\n    },\n    \"committer\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-simple-commit-schema.json
tags: []
title: SimpleCommit
---
