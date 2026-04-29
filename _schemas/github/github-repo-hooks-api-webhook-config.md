---
description: Configuration object of the webhook
layout: schema
name: webhook-config
properties_list:
- description: ''
  name: url
  type: object
- description: ''
  name: content_type
  type: object
- description: ''
  name: secret
  type: object
- description: ''
  name: insecure_ssl
  type: object
provider_name: GitHub
provider_slug: github
schema_file: json-schema/github-repo-hooks-api-webhook-config-schema.json
slug: github-repo-hooks-api-webhook-config
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-hooks-api-webhook-config-schema.json\",\n  \"title\": \"webhook-config\",\n  \"description\": \"Configuration object of the webhook\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"url\": {\n      \"$ref\": \"#/components/schemas/webhook-config-url\"\n    },\n    \"content_type\": {\n      \"$ref\": \"#/components/schemas/webhook-config-content-type\"\n    },\n    \"secret\": {\n      \"$ref\": \"#/components/schemas/webhook-config-secret\"\n    },\n    \"insecure_ssl\": {\n      \"$ref\": \"#/components/schemas/webhook-config-insecure-ssl\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github/refs/heads/main/json-schema/github-repo-hooks-api-webhook-config-schema.json
tags:
- Code
- Pipelines
- Platform
- Software Development
- Source Control
- T1
title: webhook-config
---
