---
description: ''
layout: schema
name: TokenResponse
properties_list:
- description: JWT access token
  name: access_token
  type: string
- description: Token type (Bearer)
  name: token_type
  type: string
- description: Token expiry in seconds
  name: expires_in
  type: integer
provider_name: Basiq
provider_slug: basiq
schema_file: json-schema/tokenresponse.json
slug: tokenresponse
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/tokenresponse.json\",\n  \"title\": \"TokenResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"JWT access token\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"Token type (Bearer)\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Token expiry in seconds\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basiq/refs/heads/main/json-schema/tokenresponse.json
tags:
- Australia
- Banking
- CDR
- Financial Data
- Fintech
- Open Banking
- Transactions
title: TokenResponse
---
