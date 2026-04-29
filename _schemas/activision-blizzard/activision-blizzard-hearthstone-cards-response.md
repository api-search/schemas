---
description: Paginated Hearthstone cards response
layout: schema
name: HearthstoneCardsResponse
properties_list:
- description: List of cards
  name: cards
  type: array
- description: Total card count
  name: cardCount
  type: integer
- description: Total page count
  name: pageCount
  type: integer
- description: Current page
  name: page
  type: integer
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-hearthstone-cards-response-schema.json
slug: activision-blizzard-hearthstone-cards-response
source_filename: activision-blizzard-hearthstone-cards-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-hearthstone-cards-response-schema.json\",\n  \"title\": \"HearthstoneCardsResponse\",\n  \"description\": \"Paginated Hearthstone cards response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cards\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/HearthstoneCard\"\n      },\n      \"description\": \"List of cards\"\n    },\n    \"cardCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total card count\",\n      \"example\": 2847\n    },\n    \"pageCount\": {\n      \"type\": \"integer\",\n      \"description\": \"Total page count\",\n      \"example\": 143\n    },\n    \"page\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page\",\n      \"example\": 1\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-hearthstone-cards-response-schema.json
tags: []
title: HearthstoneCardsResponse
---
