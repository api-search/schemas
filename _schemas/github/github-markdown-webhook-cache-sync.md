---
description: webhook-cache-sync from GitHub API
layout: schema
name: webhook-cache-sync
properties_list:
- description: ''
  name: after
  type: string
- description: ''
  name: before
  type: string
- description: ''
  name: cache_location
  type: string
- description: ''
  name: enterprise
  type: object
- description: ''
  name: installation
  type: object
- description: ''
  name: organization
  type: object
- description: ''
  name: ref
  type: string
- description: ''
  name: repository
  type: object
- description: ''
  name: sender
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-markdown-webhook-cache-sync-schema.json
slug: github-markdown-webhook-cache-sync
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-markdown-webhook-cache-sync-schema.json\",\n  \"title\": \"webhook-cache-sync\",\n  \"description\": \"webhook-cache-sync from GitHub API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"after\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"before\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cache_location\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"enterprise\": {\n      \"$ref\": \"#/components/schemas/enterprise-webhooks\"\n    },\n    \"installation\": {\n      \"$ref\": \"#/components/schemas/simple-installation\"\n    },\n    \"organization\": {\n      \"$ref\": \"#/components/schemas/organization-simple-webhooks\"\n    },\n    \"ref\": {\n      \"type\": \"string\",\n\
  \      \"example\": \"main\"\n    },\n    \"repository\": {\n      \"$ref\": \"#/components/schemas/repository-webhooks\"\n    },\n    \"sender\": {\n      \"$ref\": \"#/components/schemas/simple-user-webhooks\"\n    }\n  },\n  \"required\": [\n    \"cache_location\",\n    \"ref\",\n    \"before\",\n    \"after\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-markdown-webhook-cache-sync-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: webhook-cache-sync
---
