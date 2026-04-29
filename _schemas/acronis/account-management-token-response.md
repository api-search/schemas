---
description: OAuth2 token response
layout: schema
name: TokenResponse
properties_list:
- description: JWT access token
  name: access_token
  type: string
- description: ''
  name: token_type
  type: string
- description: Token lifetime in seconds
  name: expires_in
  type: integer
- description: Refresh token for obtaining new access tokens
  name: refresh_token
  type: string
- description: Granted OAuth2 scopes
  name: scope
  type: string
provider_name: Acronis
provider_slug: acronis
schema_file: json-schema/account-management-token-response-schema.json
slug: account-management-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-token-response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"description\": \"OAuth2 token response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"JWT access token\",\n      \"example\": \"eyJhbGciOiJSUzI1NiIsInR5cCI6IkpXVCJ9...\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Bearer\"\n      ],\n      \"example\": \"Bearer\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Token lifetime in seconds\",\n      \"example\": 3600\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"Refresh token for obtaining new access tokens\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"\
  description\": \"Granted OAuth2 scopes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/acronis/refs/heads/main/json-schema/account-management-token-response-schema.json
tags:
- Cybersecurity
- Data Protection
- Endpoint Management
title: TokenResponse
---
