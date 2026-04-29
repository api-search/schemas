---
description: OAuth 2.0 token request using client credentials
layout: schema
name: OAuthTokenRequest
properties_list:
- description: OAuth grant type
  name: grant_type
  type: string
- description: OAuth client ID
  name: client_id
  type: string
- description: OAuth client secret
  name: client_secret
  type: string
provider_name: Abacus
provider_slug: abacus
schema_file: json-schema/abacus-oauth-token-request-schema.json
slug: abacus-oauth-token-request
source_filename: abacus-oauth-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-oauth-token-request-schema.json\",\n  \"title\": \"OAuthTokenRequest\",\n  \"description\": \"OAuth 2.0 token request using client credentials\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grant_type\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth grant type\",\n      \"enum\": [\n        \"client_credentials\"\n      ],\n      \"example\": \"client_credentials\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth client ID\",\n      \"example\": \"example-client-id\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth client secret\",\n      \"example\": \"example-client-secret\"\n    }\n  },\n  \"required\": [\n    \"grant_type\",\n    \"client_id\",\n    \"client_secret\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/abacus/refs/heads/main/json-schema/abacus-oauth-token-request-schema.json
tags:
- Accounting
- Expense Management
- Finance
- Reimbursement
title: OAuthTokenRequest
---
