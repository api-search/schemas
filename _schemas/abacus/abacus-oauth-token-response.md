---
description: OAuth 2.0 access token response
layout: schema
name: OAuthTokenResponse
properties_list:
- description: Access token for API requests
  name: access_token
  type: string
- description: Token type (always Bearer)
  name: token_type
  type: string
- description: Token expiration time in seconds
  name: expires_in
  type: integer
provider_name: Abacus
provider_slug: abacus
schema_file: json-schema/abacus-oauth-token-response-schema.json
slug: abacus-oauth-token-response
source_filename: abacus-oauth-token-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-oauth-token-response-schema.json\",\n  \"title\": \"OAuthTokenResponse\",\n  \"description\": \"OAuth 2.0 access token response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"Access token for API requests\",\n      \"example\": \"a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"Token type (always Bearer)\",\n      \"example\": \"Bearer\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Token expiration time in seconds\",\n      \"example\": 3600\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-oauth-token-response-schema.json
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
title: OAuthTokenResponse
---
