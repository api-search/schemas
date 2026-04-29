---
description: ''
layout: schema
name: AuthenticationToken
properties_list:
- description: ''
  name: token
  type: string
- description: ''
  name: expires_at
  type: string
provider_name: GitHub Actions
provider_slug: github-actions
schema_file: json-schema/github-actions-authentication-token-schema.json
slug: github-actions-authentication-token
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AuthenticationToken\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"token\": {\n      \"type\": \"string\"\n    },\n    \"expires_at\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/github-actions/refs/heads/main/json-schema/github-actions-authentication-token-schema.json
tags: []
title: AuthenticationToken
---
