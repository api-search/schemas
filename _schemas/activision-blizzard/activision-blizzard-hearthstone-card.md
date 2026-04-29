---
description: A Hearthstone card
layout: schema
name: HearthstoneCard
properties_list:
- description: Card ID
  name: id
  type: integer
- description: Whether the card is collectible (1=yes)
  name: collectible
  type: integer
- description: Card slug
  name: slug
  type: string
- description: Class ID
  name: classId
  type: integer
- description: Multi-class IDs
  name: multiClassIds
  type: array
- description: Card type ID
  name: cardTypeId
  type: integer
- description: Card set ID
  name: cardSetId
  type: integer
- description: Rarity ID
  name: rarityId
  type: integer
- description: Artist name
  name: artistName
  type: string
- description: Card health
  name: health
  type: integer
- description: Card attack
  name: attack
  type: integer
- description: Mana cost
  name: manaCost
  type: integer
- description: Card name
  name: name
  type: string
- description: Card text
  name: text
  type: string
- description: Card image URL
  name: image
  type: string
- description: Gold card image URL
  name: imageGold
  type: string
- description: Card flavor text
  name: flavorText
  type: string
- description: Cropped card image URL
  name: cropImage
  type: string
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-hearthstone-card-schema.json
slug: activision-blizzard-hearthstone-card
source_filename: activision-blizzard-hearthstone-card-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-hearthstone-card-schema.json\",\n  \"title\": \"HearthstoneCard\",\n  \"description\": \"A Hearthstone card\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Card ID\",\n      \"example\": 1234\n    },\n    \"collectible\": {\n      \"type\": \"integer\",\n      \"description\": \"Whether the card is collectible (1=yes)\",\n      \"example\": 1\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"Card slug\",\n      \"example\": \"ragnaros-the-firelord\"\n    },\n    \"classId\": {\n      \"type\": \"integer\",\n      \"description\": \"Class ID\",\n      \"example\": 1\n    },\n    \"multiClassIds\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"integer\"\n\
  \      },\n      \"description\": \"Multi-class IDs\"\n    },\n    \"cardTypeId\": {\n      \"type\": \"integer\",\n      \"description\": \"Card type ID\",\n      \"example\": 4\n    },\n    \"cardSetId\": {\n      \"type\": \"integer\",\n      \"description\": \"Card set ID\",\n      \"example\": 2\n    },\n    \"rarityId\": {\n      \"type\": \"integer\",\n      \"description\": \"Rarity ID\",\n      \"example\": 5\n    },\n    \"artistName\": {\n      \"type\": \"string\",\n      \"description\": \"Artist name\",\n      \"example\": \"Alex Horley\"\n    },\n    \"health\": {\n      \"type\": \"integer\",\n      \"description\": \"Card health\",\n      \"example\": 8\n    },\n    \"attack\": {\n      \"type\": \"integer\",\n      \"description\": \"Card attack\",\n      \"example\": 8\n    },\n    \"manaCost\": {\n      \"type\": \"integer\",\n      \"description\": \"Mana cost\",\n      \"example\": 8\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"\
  Card name\",\n      \"example\": \"Ragnaros the Firelord\"\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"Card text\"\n    },\n    \"image\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Card image URL\"\n    },\n    \"imageGold\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Gold card image URL\"\n    },\n    \"flavorText\": {\n      \"type\": \"string\",\n      \"description\": \"Card flavor text\"\n    },\n    \"cropImage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"Cropped card image URL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-hearthstone-card-schema.json
tags: []
title: HearthstoneCard
---
