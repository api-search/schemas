---
description: Diablo III career profile
layout: schema
name: D3CareerProfile
properties_list:
- description: Player BattleTag
  name: battletag
  type: string
- description: Paragon level
  name: paragonLevel
  type: integer
- description: Hardcore paragon level
  name: paragonLevelHardcore
  type: integer
- description: Guild name
  name: guildName
  type: string
- description: List of heroes
  name: heroes
  type: array
- description: ID of last hero played
  name: lastHeroPlayed
  type: integer
- description: Kill statistics
  name: kills
  type: object
- description: Time played by class
  name: timePlayed
  type: object
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-d3-career-profile-schema.json
slug: activision-blizzard-d3-career-profile
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-d3-career-profile-schema.json\",\n  \"title\": \"D3CareerProfile\",\n  \"description\": \"Diablo III career profile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"battletag\": {\n      \"type\": \"string\",\n      \"description\": \"Player BattleTag\",\n      \"example\": \"Player#1234\"\n    },\n    \"paragonLevel\": {\n      \"type\": \"integer\",\n      \"description\": \"Paragon level\",\n      \"example\": 1500\n    },\n    \"paragonLevelHardcore\": {\n      \"type\": \"integer\",\n      \"description\": \"Hardcore paragon level\",\n      \"example\": 200\n    },\n    \"guildName\": {\n      \"type\": \"string\",\n      \"description\": \"Guild name\"\n    },\n    \"heroes\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/D3HeroSummary\"\
  \n      },\n      \"description\": \"List of heroes\"\n    },\n    \"lastHeroPlayed\": {\n      \"type\": \"integer\",\n      \"description\": \"ID of last hero played\",\n      \"example\": 12345\n    },\n    \"kills\": {\n      \"type\": \"object\",\n      \"description\": \"Kill statistics\"\n    },\n    \"timePlayed\": {\n      \"type\": \"object\",\n      \"description\": \"Time played by class\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-d3-career-profile-schema.json
tags: []
title: D3CareerProfile
---
