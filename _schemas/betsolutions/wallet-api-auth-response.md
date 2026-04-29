---
description: Authentication response with private player token.
layout: schema
name: AuthResponse
properties_list:
- description: Whether authentication succeeded.
  name: success
  type: boolean
- description: Private player token for subsequent API calls.
  name: token
  type: string
- description: Unique player identifier.
  name: playerId
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-auth-response-schema.json
slug: wallet-api-auth-response
source_filename: wallet-api-auth-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-auth-response-schema.json\",\n  \"title\": \"AuthResponse\",\n  \"description\": \"Authentication response with private player token.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether authentication succeeded.\",\n      \"example\": true\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"Private player token for subsequent API calls.\",\n      \"example\": \"priv-token-xyz789\"\n    },\n    \"playerId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique player identifier.\",\n      \"example\": \"player-500123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-auth-response-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: AuthResponse
---
