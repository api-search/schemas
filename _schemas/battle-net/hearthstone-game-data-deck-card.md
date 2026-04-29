---
description: A card included in a deck.
layout: schema
name: DeckCard
properties_list:
- description: The card ID.
  name: id
  type: integer
- description: Number of copies of this card in the deck.
  name: count
  type: integer
- description: The card slug.
  name: slug
  type: string
- description: The card name.
  name: name
  type: string
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-deck-card-schema.json
slug: hearthstone-game-data-deck-card
source_filename: hearthstone-game-data-deck-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-deck-card-schema.json\",\n  \"title\": \"DeckCard\",\n  \"description\": \"A card included in a deck.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The card ID.\",\n      \"example\": 52119\n    },\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of copies of this card in the deck.\",\n      \"example\": 2\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The card slug.\",\n      \"example\": \"52119-ragnaros-the-firelord\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The card name.\",\n      \"example\": \"Ragnaros the Firelord\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-deck-card-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: DeckCard
---
