---
description: TokenResponse schema from AT&T API
layout: schema
name: TokenResponse
properties_list:
- description: OAuth access token valid for 2 days (172800 seconds)
  name: access_token
  type: string
- description: Token expiration time in seconds (default 172800)
  name: expires_in
  type: integer
- description: Refresh token valid for 90 days
  name: refresh_token
  type: string
- description: Token type (always BEARER)
  name: token_type
  type: string
provider_name: AT&T
provider_slug: at-and-t
schema_file: json-schema/sms-api-token-response-schema.json
slug: sms-api-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-token-response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"description\": \"TokenResponse schema from AT&T API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth access token valid for 2 days (172800 seconds)\",\n      \"example\": \"a1b2c3d4e5f6a1b2c3d4e5f6a1b2c3d4\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Token expiration time in seconds (default 172800)\",\n      \"example\": 172800\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"Refresh token valid for 90 days\",\n      \"example\": \"f6e5d4c3b2a1f6e5d4c3b2a1f6e5d4c3\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"Token type (always\
  \ BEARER)\",\n      \"example\": \"BEARER\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/json-schema/sms-api-token-response-schema.json
tags:
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
title: TokenResponse
---
