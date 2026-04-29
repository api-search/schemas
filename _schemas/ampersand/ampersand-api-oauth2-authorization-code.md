---
description: Oauth2AuthorizationCode schema from Ampersand API
layout: schema
name: Oauth2AuthorizationCode
properties_list:
- description: The access token for the connection.
  name: accessToken
  type: object
- description: The refresh token to use for the connection.
  name: refreshToken
  type: object
- description: The scopes for the tokens.
  name: scopes
  type: array
provider_name: Ampersand
provider_slug: ampersand
schema_file: json-schema/ampersand-api-oauth2-authorization-code-schema.json
slug: ampersand-api-oauth2-authorization-code
source_filename: ampersand-api-oauth2-authorization-code-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-oauth2-authorization-code-schema.json\",\n  \"title\": \"Oauth2AuthorizationCode\",\n  \"description\": \"Oauth2AuthorizationCode schema from Ampersand API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessToken\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"token\"\n      ],\n      \"description\": \"The access token for the connection.\",\n      \"properties\": {\n        \"token\": {\n          \"type\": \"string\"\n        },\n        \"expiresAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"issuedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"refreshToken\": {\n      \"type\": \"object\",\n      \"required\": [\n        \"token\"\n      ],\n\
  \      \"description\": \"The refresh token to use for the connection.\",\n      \"properties\": {\n        \"token\": {\n          \"type\": \"string\"\n        },\n        \"expiresAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        },\n        \"issuedAt\": {\n          \"type\": \"string\",\n          \"format\": \"date-time\"\n        }\n      }\n    },\n    \"scopes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The scopes for the tokens.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/ampersand/refs/heads/main/json-schema/ampersand-api-oauth2-authorization-code-schema.json
tags:
- Developer Tools
- Integrations
- Platform
- SaaS
- OAuth
- Data Sync
- Webhooks
title: Oauth2AuthorizationCode
---
