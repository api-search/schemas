---
description: JWT token data returned after successful authentication.
layout: schema
name: TokenData
properties_list:
- description: JWT access token for Bearer authentication.
  name: access_token
  type: string
- description: Token type, always Bearer.
  name: token_type
  type: string
- description: Token expiry duration in seconds.
  name: expires_in
  type: string
- description: Refresh token for obtaining new access tokens.
  name: refresh_token
  type: string
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-token-data-schema.json
slug: apache-ofbiz-token-data
source_filename: apache-ofbiz-token-data-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-token-data-schema.json\",\n  \"title\": \"TokenData\",\n  \"description\": \"JWT token data returned after successful authentication.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"JWT access token for Bearer authentication.\",\n      \"example\": \"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.example\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"Token type, always Bearer.\",\n      \"example\": \"Bearer\"\n    },\n    \"expires_in\": {\n      \"type\": \"string\",\n      \"description\": \"Token expiry duration in seconds.\",\n      \"example\": \"1800\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"Refresh token for obtaining new access\
  \ tokens.\",\n      \"example\": \"dGhpc19pc19hX3JlZnJlc2hfdG9rZW4\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-token-data-schema.json
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: TokenData
---
