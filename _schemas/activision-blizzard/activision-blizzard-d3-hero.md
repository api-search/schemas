---
description: A Diablo III hero
layout: schema
name: D3Hero
properties_list:
- description: Hero ID
  name: id
  type: integer
- description: Hero name
  name: name
  type: string
- description: Hero class
  name: class
  type: string
- description: Hero gender (0=male, 1=female)
  name: gender
  type: integer
- description: Hero level
  name: level
  type: integer
- description: Paragon level
  name: paragonLevel
  type: integer
- description: Whether this is a hardcore hero
  name: hardcore
  type: boolean
- description: Whether this is a seasonal hero
  name: seasonal
  type: boolean
- description: Whether this hero is dead
  name: dead
  type: boolean
- description: Kill statistics
  name: kills
  type: object
- description: Hero skills and runes
  name: skills
  type: object
- description: Equipped items
  name: items
  type: object
- description: Character stats
  name: stats
  type: object
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-d3-hero-schema.json
slug: activision-blizzard-d3-hero
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-d3-hero-schema.json\",\n  \"title\": \"D3Hero\",\n  \"description\": \"A Diablo III hero\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Hero ID\",\n      \"example\": 12345\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hero name\",\n      \"example\": \"Zul'jin\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"Hero class\",\n      \"example\": \"barbarian\"\n    },\n    \"gender\": {\n      \"type\": \"integer\",\n      \"description\": \"Hero gender (0=male, 1=female)\",\n      \"example\": 0\n    },\n    \"level\": {\n      \"type\": \"integer\",\n      \"description\": \"Hero level\",\n      \"example\": 70\n    },\n    \"paragonLevel\":\
  \ {\n      \"type\": \"integer\",\n      \"description\": \"Paragon level\",\n      \"example\": 1500\n    },\n    \"hardcore\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a hardcore hero\"\n    },\n    \"seasonal\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a seasonal hero\"\n    },\n    \"dead\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this hero is dead\"\n    },\n    \"kills\": {\n      \"type\": \"object\",\n      \"description\": \"Kill statistics\"\n    },\n    \"skills\": {\n      \"type\": \"object\",\n      \"description\": \"Hero skills and runes\"\n    },\n    \"items\": {\n      \"type\": \"object\",\n      \"description\": \"Equipped items\"\n    },\n    \"stats\": {\n      \"type\": \"object\",\n      \"description\": \"Character stats\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-d3-hero-schema.json
tags: []
title: D3Hero
---
