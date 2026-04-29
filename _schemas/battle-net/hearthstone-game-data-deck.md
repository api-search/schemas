---
description: A Hearthstone deck.
layout: schema
name: Deck
properties_list:
- description: The deck code string.
  name: deckCode
  type: string
- description: The deck version.
  name: version
  type: integer
- description: The deck format (standard, wild, classic).
  name: format
  type: string
- description: The class associated with a deck.
  name: class
  type: object
- description: The cards in the deck.
  name: cards
  type: array
- description: Total number of cards in the deck.
  name: cardCount
  type: integer
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-deck-schema.json
slug: hearthstone-game-data-deck
source_filename: hearthstone-game-data-deck-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-deck-schema.json\",\n  \"title\": \"Deck\",\n  \"description\": \"A Hearthstone deck.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"deckCode\": {\n      \"type\": \"string\",\n      \"description\": \"The deck code string.\",\n      \"example\": \"AAECAf0EAA8A\"\n    },\n    \"version\": {\n      \"type\": \"integer\",\n      \"description\": \"The deck version.\",\n      \"example\": 1\n    },\n    \"format\": {\n      \"type\": \"string\",\n      \"description\": \"The deck format (standard, wild, classic).\",\n      \"example\": \"standard\"\n    },\n    \"class\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"slug\": {\n          \"type\": \"string\",\n          \"description\": \"The class slug.\",\n          \"example\": \"mage\"\n        },\n     \
  \   \"id\": {\n          \"type\": \"integer\",\n          \"description\": \"The class ID.\",\n          \"example\": 3\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"The class name.\",\n          \"example\": \"Mage\"\n        }\n      },\n      \"description\": \"The class associated with a deck.\"\n    },\n    \"cards\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The card ID.\",\n            \"example\": 52119\n          },\n          \"count\": {\n            \"type\": \"integer\",\n            \"description\": \"Number of copies of this card in the deck.\",\n            \"example\": 2\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"The card slug.\",\n            \"example\": \"52119-ragnaros-the-firelord\"\n          },\n   \
  \       \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The card name.\",\n            \"example\": \"Ragnaros the Firelord\"\n          }\n        },\n        \"description\": \"A card included in a deck.\"\n      },\n      \"description\": \"The cards in the deck.\"\n    },\n    \"cardCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of cards in the deck.\",\n      \"example\": 30\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-deck-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: Deck
---
