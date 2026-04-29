---
description: Standard API response containing JWT token data.
layout: schema
name: TokenResponse
properties_list:
- description: HTTP status code.
  name: statusCode
  type: integer
- description: Human-readable status description.
  name: statusDescription
  type: string
- description: Success message from the server.
  name: successMessage
  type: string
- description: JWT token data returned after successful authentication.
  name: data
  type: object
provider_name: Apache OFBiz
provider_slug: apache-ofbiz
schema_file: json-schema/apache-ofbiz-token-response-schema.json
slug: apache-ofbiz-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-token-response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"description\": \"Standard API response containing JWT token data.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"statusCode\": {\n      \"type\": \"integer\",\n      \"description\": \"HTTP status code.\",\n      \"example\": 200\n    },\n    \"statusDescription\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable status description.\",\n      \"example\": \"OK\"\n    },\n    \"successMessage\": {\n      \"type\": \"string\",\n      \"description\": \"Success message from the server.\",\n      \"example\": \"Token granted.\"\n    },\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"JWT token data returned after successful authentication.\",\n      \"properties\": {\n      \
  \  \"access_token\": {\n          \"type\": \"string\",\n          \"description\": \"JWT access token for Bearer authentication.\",\n          \"example\": \"eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzUxMiJ9.example\"\n        },\n        \"token_type\": {\n          \"type\": \"string\",\n          \"description\": \"Token type, always Bearer.\",\n          \"example\": \"Bearer\"\n        },\n        \"expires_in\": {\n          \"type\": \"string\",\n          \"description\": \"Token expiry duration in seconds.\",\n          \"example\": \"1800\"\n        },\n        \"refresh_token\": {\n          \"type\": \"string\",\n          \"description\": \"Refresh token for obtaining new access tokens.\",\n          \"example\": \"dGhpc19pc19hX3JlZnJlc2hfdG9rZW4\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-ofbiz/refs/heads/main/json-schema/apache-ofbiz-token-response-schema.json
tags:
- ERP
- CRM
- E-Commerce
- Business Applications
- Apache
- Java
- Open Source
- Supply Chain
title: TokenResponse
---
