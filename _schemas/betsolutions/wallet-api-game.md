---
description: A BetSolutions game with product metadata.
layout: schema
name: Game
properties_list:
- description: Unique game identifier.
  name: gameId
  type: string
- description: Product category ID (1=Table Games, 2=Slots, 3=Provably Fair).
  name: productId
  type: integer
- description: Game display name.
  name: name
  type: string
- description: Whether the game supports freespin/freeplay campaigns.
  name: hasFreePay
  type: boolean
- description: URL to launch the game.
  name: launchUrl
  type: string
- description: Return-to-player percentage.
  name: rtp
  type: number
- description: Rake percentage for the game.
  name: rakePercent
  type: number
provider_name: BetSolutions
provider_slug: betsolutions
schema_file: json-schema/wallet-api-game-schema.json
slug: wallet-api-game
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-game-schema.json\",\n  \"title\": \"Game\",\n  \"description\": \"A BetSolutions game with product metadata.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"gameId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique game identifier.\",\n      \"example\": \"game-001\"\n    },\n    \"productId\": {\n      \"type\": \"integer\",\n      \"description\": \"Product category ID (1=Table Games, 2=Slots, 3=Provably Fair).\",\n      \"example\": 2\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Game display name.\",\n      \"example\": \"Book of Ra\"\n    },\n    \"hasFreePay\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the game supports freespin/freeplay campaigns.\",\n      \"example\": true\n    },\n    \"launchUrl\": {\n\
  \      \"type\": \"string\",\n      \"description\": \"URL to launch the game.\",\n      \"example\": \"https://games.betsolutions.com/slots/book-of-ra\"\n    },\n    \"rtp\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Return-to-player percentage.\",\n      \"example\": 96.0\n    },\n    \"rakePercent\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Rake percentage for the game.\",\n      \"example\": 3.5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/betsolutions/refs/heads/main/json-schema/wallet-api-game-schema.json
tags:
- Betting
- Casinos
- Gaming
- Gambling
- Slots
- Sports Betting
title: Game
---
