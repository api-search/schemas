---
description: Request body for retrieving the available game list.
layout: schema
name: GameListRequest
properties_list:
- description: The merchant's unique identifier.
  name: merchantId
  type: string
- description: SHA-256 hash for request authentication.
  name: hash
  type: string
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-game-list-request-schema.json
slug: wallet-api-game-list-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-game-list-request-schema.json\",\n  \"title\": \"GameListRequest\",\n  \"description\": \"Request body for retrieving the available game list.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"merchantId\": {\n      \"type\": \"string\",\n      \"description\": \"The merchant's unique identifier.\",\n      \"example\": \"merchant-001\"\n    },\n    \"hash\": {\n      \"type\": \"string\",\n      \"description\": \"SHA-256 hash for request authentication.\",\n      \"example\": \"d4e5f6g7...\"\n    }\n  },\n  \"required\": [\n    \"merchantId\",\n    \"hash\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-game-list-request-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: GameListRequest
---
