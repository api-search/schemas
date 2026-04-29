---
description: TokenResponse schema from Avalara API
layout: schema
name: TokenResponse
properties_list:
- description: The OAuth 2.0 access token
  name: access_token
  type: string
- description: ''
  name: token_type
  type: string
- description: Token expiry time in seconds
  name: expires_in
  type: integer
- description: Granted scopes
  name: scope
  type: string
- description: Refresh token (if applicable)
  name: refresh_token
  type: string
provider_name: Avalara
provider_slug: avalara
schema_file: json-schema/portal-oauth-token-response-schema.json
slug: portal-oauth-token-response
source_filename: portal-oauth-token-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/portal-oauth-token-response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"description\": \"TokenResponse schema from Avalara API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"The OAuth 2.0 access token\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"Bearer\"\n      ]\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Token expiry time in seconds\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Granted scopes\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"Refresh token (if applicable)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/avalara/refs/heads/main/json-schema/portal-oauth-token-response-schema.json
tags:
- Taxes
title: TokenResponse
---
