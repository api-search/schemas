---
description: An API access token returned after successful authentication
layout: schema
name: AccessToken
properties_list:
- description: The OAuth2 access token string
  name: access_token
  type: string
- description: Token type, always 'Bearer'
  name: token_type
  type: string
- description: Number of seconds until the token expires
  name: expires_in
  type: integer
- description: Refresh token (not used in API client credential flow)
  name: refresh_token
  type: string
provider_name: Looker
provider_slug: looker
schema_file: json-schema/looker-access-token-schema.json
slug: looker-access-token
source_filename: looker-access-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccessToken\",\n  \"type\": \"object\",\n  \"description\": \"An API access token returned after successful authentication\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"The OAuth2 access token string\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"Token type, always 'Bearer'\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of seconds until the token expires\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"Refresh token (not used in API client credential flow)\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/looker/refs/heads/main/json-schema/looker-access-token-schema.json
tags:
- Analytics
- BI Platform
- Business Intelligence
- Data Analytics
- Data Visualization
title: AccessToken
---
