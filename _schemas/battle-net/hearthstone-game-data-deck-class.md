---
description: The class associated with a deck.
layout: schema
name: DeckClass
properties_list:
- description: The class slug.
  name: slug
  type: string
- description: The class ID.
  name: id
  type: integer
- description: The class name.
  name: name
  type: string
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-deck-class-schema.json
slug: hearthstone-game-data-deck-class
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-deck-class-schema.json\",\n  \"title\": \"DeckClass\",\n  \"description\": \"The class associated with a deck.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The class slug.\",\n      \"example\": \"mage\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The class ID.\",\n      \"example\": 3\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The class name.\",\n      \"example\": \"Mage\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-deck-class-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: DeckClass
---
