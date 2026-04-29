---
description: A Hearthstone deck
layout: schema
name: HearthstoneDeck
properties_list:
- description: The deck code
  name: deckCode
  type: string
- description: Deck format version
  name: version
  type: integer
- description: Deck format
  name: format
  type: object
- description: ''
  name: hero
  type: object
- description: ''
  name: heroPower
  type: object
- description: Deck class
  name: class
  type: object
- description: Cards in the deck
  name: cards
  type: array
- description: Number of cards in the deck
  name: cardCount
  type: integer
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-hearthstone-deck-schema.json
slug: activision-blizzard-hearthstone-deck
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-hearthstone-deck-schema.json\",\n  \"title\": \"HearthstoneDeck\",\n  \"description\": \"A Hearthstone deck\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deckCode\": {\n      \"type\": \"string\",\n      \"description\": \"The deck code\",\n      \"example\": \"AAECAQcG0LQDubQD3rUD57UDibYDvbYDDI...\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"Deck format version\",\n      \"example\": 1\n    },\n    \"format\": {\n      \"type\": \"object\",\n      \"description\": \"Deck format\"\n    },\n    \"hero\": {\n      \"$ref\": \"#/components/schemas/HearthstoneCard\"\n    },\n    \"heroPower\": {\n      \"$ref\": \"#/components/schemas/HearthstoneCard\"\n    },\n    \"class\": {\n      \"type\": \"object\",\n      \"description\": \"\
  Deck class\"\n    },\n    \"cards\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HearthstoneCard\"\n      },\n      \"description\": \"Cards in the deck\"\n    },\n    \"cardCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of cards in the deck\",\n      \"example\": 30\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-hearthstone-deck-schema.json
tags: []
title: HearthstoneDeck
---
