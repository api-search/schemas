---
description: A paginated list of Hearthstone cards.
layout: schema
name: CardSearchResponse
properties_list:
- description: List of matching cards.
  name: cards
  type: array
- description: Total number of matching cards.
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
schema_file: json-schema/hearthstone-game-data-card-search-response-schema.json
slug: hearthstone-game-data-card-search-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-card-search-response-schema.json\",\n  \"title\": \"CardSearchResponse\",\n  \"description\": \"A paginated list of Hearthstone cards.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cards\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"description\": \"The card's unique ID.\",\n            \"example\": 52119\n          },\n          \"collectible\": {\n            \"type\": \"integer\",\n            \"description\": \"Indicates if the card is collectible (1) or uncollectible (0).\",\n            \"example\": 1\n          },\n          \"slug\": {\n            \"type\": \"string\",\n            \"description\": \"A human-readable identifier for\
  \ the card.\",\n            \"example\": \"52119-ragnaros-the-firelord\"\n          },\n          \"classId\": {\n            \"type\": \"integer\",\n            \"description\": \"The class ID of the card.\",\n            \"example\": 12\n          },\n          \"multiClassIds\": {\n            \"type\": \"array\",\n            \"items\": {},\n            \"description\": \"Class IDs if the card belongs to multiple classes.\"\n          },\n          \"cardTypeId\": {\n            \"type\": \"integer\",\n            \"description\": \"The card type ID.\",\n            \"example\": 4\n          },\n          \"cardSetId\": {\n            \"type\": \"integer\",\n            \"description\": \"The set ID of the card.\",\n            \"example\": 3\n          },\n          \"rarityId\": {\n            \"type\": \"integer\",\n            \"description\": \"The rarity ID of the card.\",\n            \"example\": 5\n          },\n          \"artistName\": {\n            \"type\": \"string\"\
  ,\n            \"description\": \"The name of the card's artist.\",\n            \"example\": \"Alex Horley Orlandelli\"\n          },\n          \"health\": {\n            \"type\": \"integer\",\n            \"description\": \"The health of the minion.\",\n            \"example\": 8\n          },\n          \"attack\": {\n            \"type\": \"integer\",\n            \"description\": \"The attack power of the card.\",\n            \"example\": 8\n          },\n          \"manaCost\": {\n            \"type\": \"integer\",\n            \"description\": \"The mana cost to play the card.\",\n            \"example\": 8\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"description\": \"The name of the card.\",\n            \"example\": \"Ragnaros the Firelord\"\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"description\": \"The card's text.\",\n            \"example\": \"Can't attack. At the end of your turn, deal\
  \ 8 damage to a random enemy.\"\n          },\n          \"image\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL of the card image.\",\n            \"example\": \"https://d15f34w2p8l1cc.cloudfront.net/hearthstone/bf5f0b3ef6d61b6bec59a7a7a1d95b8f0d9d74d2.png\"\n          },\n          \"flavorText\": {\n            \"type\": \"string\",\n            \"description\": \"Flavor text for the card.\",\n            \"example\": \"He was summoned by the Dark Iron dwarves.\"\n          },\n          \"cropImage\": {\n            \"type\": \"string\",\n            \"format\": \"uri\",\n            \"description\": \"URL of the cropped card image.\",\n            \"example\": \"https://d15f34w2p8l1cc.cloudfront.net/hearthstone/cropped/52119.jpg\"\n          },\n          \"childIds\": {\n            \"type\": \"array\",\n            \"items\": {},\n            \"description\": \"IDs of child cards.\"\n          }\n        },\n        \"\
  description\": \"A Hearthstone card object.\"\n      },\n      \"description\": \"List of matching cards.\"\n    },\n    \"cardCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of matching cards.\",\n      \"example\": 100\n    },\n    \"pageCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of pages.\",\n      \"example\": 5\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number.\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-card-search-response-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: CardSearchResponse
---
