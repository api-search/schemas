---
description: webhook-check-run-created from GitHub API
layout: schema
name: webhook-check-run-created
properties_list:
- description: ''
  name: action
  type: string
- description: ''
  name: check_run
  type: object
- description: ''
  name: installation
  type: object
- description: ''
  name: organization
  type: object
- description: ''
  name: repository
  type: object
- description: ''
  name: sender
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-markdown-webhook-check-run-created-schema.json
slug: github-markdown-webhook-check-run-created
source_filename: github-markdown-webhook-check-run-created-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-markdown-webhook-check-run-created-schema.json\",\n  \"title\": \"webhook-check-run-created\",\n  \"description\": \"webhook-check-run-created from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"action\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"created\"\n      ],\n      \"example\": \"created\"\n    },\n    \"check_run\": {\n      \"$ref\": \"#/components/schemas/check-run-with-simple-check-suite\"\n    },\n    \"installation\": {\n      \"$ref\": \"#/components/schemas/simple-installation\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/components/schemas/organization-simple-webhooks\"\n    },\n    \"repository\": {\n      \"$ref\": \"#/components/schemas/repository-webhooks\"\n    },\n    \"sender\": {\n      \"$ref\": \"#/components/schemas/simple-user-webhooks\"\
  \n    }\n  },\n  \"required\": [\n    \"check_run\",\n    \"repository\",\n    \"sender\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-markdown-webhook-check-run-created-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: webhook-check-run-created
---
