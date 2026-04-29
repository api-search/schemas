---
description: Response containing available games and product metadata.
layout: schema
name: GameListResponse
properties_list:
- description: Whether the request succeeded.
  name: success
  type: boolean
- description: Array of available game products.
  name: products
  type: array
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-game-list-response-schema.json
slug: wallet-api-game-list-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-game-list-response-schema.json\",\n  \"title\": \"GameListResponse\",\n  \"description\": \"Response containing available games and product metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the request succeeded.\",\n      \"example\": true\n    },\n    \"products\": {\n      \"type\": \"array\",\n      \"description\": \"Array of available game products.\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Game\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-game-list-response-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: GameListResponse
---
