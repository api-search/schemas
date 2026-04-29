---
description: A generic metadata item.
layout: schema
name: MetadataItem
properties_list:
- description: The unique ID of the metadata item.
  name: id
  type: integer
- description: The name of the metadata item.
  name: name
  type: string
- description: The slug identifier.
  name: slug
  type: string
provider_name: Battle.net
provider_slug: battle-net
schema_file: json-schema/hearthstone-game-data-metadata-item-schema.json
slug: hearthstone-game-data-metadata-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-metadata-item-schema.json\",\n  \"title\": \"MetadataItem\",\n  \"description\": \"A generic metadata item.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"The unique ID of the metadata item.\",\n      \"example\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the metadata item.\",\n      \"example\": \"Basic\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"The slug identifier.\",\n      \"example\": \"basic\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/battle-net/refs/heads/main/json-schema/hearthstone-game-data-metadata-item-schema.json
tags:
- Games
- Gaming
- Blizzard
- World Of Warcraft
- Diablo
- Hearthstone
- Starcraft
title: MetadataItem
---
