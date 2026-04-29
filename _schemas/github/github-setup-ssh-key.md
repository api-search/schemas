---
description: ssh-key from GitHub API
layout: schema
name: ssh-key
properties_list:
- description: ''
  name: key
  type: string
- description: ''
  name: pretty-print
  type: string
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-setup-ssh-key-schema.json
slug: github-setup-ssh-key
source_filename: github-setup-ssh-key-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-setup-ssh-key-schema.json\",\n  \"title\": \"ssh-key\",\n  \"description\": \"ssh-key from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"key\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"pretty-print\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-setup-ssh-key-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: ssh-key
---
