---
description: A Hearthstone card back object.
layout: schema
name: CardBack
properties_list:
- description: The unique ID of the card back.
  name: id
  type: integer
- description: The sort category.
  name: sortCategory
  type: integer
- description: Description of the card back.
  name: text
  type: string
- description: The name of the card back.
  name: name
  type: string
- description: URL of the card back image.
  name: image
  type: string
- description: A human-readable identifier for the card back.
  name: slug
  type: string
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-card-back-schema.json
slug: hearthstone-game-data-card-back
source_filename: hearthstone-game-data-card-back-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-card-back-schema.json\",\n  \"title\": \"CardBack\",\n  \"description\": \"A Hearthstone card back object.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique ID of the card back.\",\n      \"example\": 1\n    },\n    \"sortCategory\": {\n      \"type\": \"integer\",\n      \"description\": \"The sort category.\",\n      \"example\": 2\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the card back.\",\n      \"example\": \"The standard card back for Hearthstone.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the card back.\",\n      \"example\": \"Classic\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n   \
  \   \"format\": \"uri\",\n      \"description\": \"URL of the card back image.\",\n      \"example\": \"https://d15f34w2p8l1cc.cloudfront.net/hearthstone/card-backs/classic.png\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable identifier for the card back.\",\n      \"example\": \"classic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-card-back-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: CardBack
---
