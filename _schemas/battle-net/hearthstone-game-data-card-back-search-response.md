---
description: A paginated list of Hearthstone card backs.
layout: schema
name: CardBackSearchResponse
properties_list:
- description: List of matching card backs.
  name: cardBacks
  type: array
- description: Total number of matching card backs.
  name: cardCount
  type: integer
- description: Total number of pages.
  name: pageCount
  type: integer
- description: Current page number.
  name: page
  type: integer
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-card-back-search-response-schema.json
slug: hearthstone-game-data-card-back-search-response
source_filename: hearthstone-game-data-card-back-search-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-card-back-search-response-schema.json\",\n  \"title\": \"CardBackSearchResponse\",\n  \"description\": \"A paginated list of Hearthstone card backs.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cardBacks\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The unique ID of the card back.\",\n            \"example\": 1\n          },\n          \"sortCategory\": {\n            \"type\": \"integer\",\n            \"description\": \"The sort category.\",\n            \"example\": 2\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"description\": \"Description of the card back.\",\n            \"example\"\
  : \"The standard card back for Hearthstone.\"\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the card back.\",\n            \"example\": \"Classic\"\n          },\n          \"image\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL of the card back image.\",\n            \"example\": \"https://d15f34w2p8l1cc.cloudfront.net/hearthstone/card-backs/classic.png\"\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"A human-readable identifier for the card back.\",\n            \"example\": \"classic\"\n          }\n        },\n        \"description\": \"A Hearthstone card back object.\"\n      },\n      \"description\": \"List of matching card backs.\"\n    },\n    \"cardCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching card backs.\",\n      \"example\": 150\n    },\n   \
  \ \"pageCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of pages.\",\n      \"example\": 8\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-card-back-search-response-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: CardBackSearchResponse
---
