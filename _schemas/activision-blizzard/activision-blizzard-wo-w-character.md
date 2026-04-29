---
description: Full World of Warcraft character profile
layout: schema
name: WoWCharacter
properties_list:
- description: Character ID
  name: id
  type: integer
- description: Character name
  name: name
  type: string
- description: Character gender
  name: gender
  type: object
- description: Character faction
  name: faction
  type: object
- description: Character race
  name: race
  type: object
- description: Character class
  name: character_class
  type: object
- description: Active specialization
  name: active_spec
  type: object
- description: ''
  name: realm
  type: object
- description: ''
  name: guild
  type: object
- description: Character level
  name: level
  type: integer
- description: Character experience points
  name: experience
  type: integer
- description: Total achievement points
  name: achievement_points
  type: integer
- description: Unix timestamp of last login
  name: last_login_timestamp
  type: integer
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-character-schema.json
slug: activision-blizzard-wo-w-character
source_filename: activision-blizzard-wo-w-character-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-character-schema.json\",\n  \"title\": \"WoWCharacter\",\n  \"description\": \"Full World of Warcraft character profile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Character ID\",\n      \"example\": 123456\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Character name\",\n      \"example\": \"Thrall\"\n    },\n    \"gender\": {\n      \"type\": \"object\",\n      \"description\": \"Character gender\"\n    },\n    \"faction\": {\n      \"type\": \"object\",\n      \"description\": \"Character faction\"\n    },\n    \"race\": {\n      \"type\": \"object\",\n      \"description\": \"Character race\"\n    },\n    \"character_class\": {\n      \"type\": \"object\",\n    \
  \  \"description\": \"Character class\"\n    },\n    \"active_spec\": {\n      \"type\": \"object\",\n      \"description\": \"Active specialization\"\n    },\n    \"realm\": {\n      \"$ref\": \"#/components/schemas/WoWRealm\"\n    },\n    \"guild\": {\n      \"$ref\": \"#/components/schemas/WoWGuild\"\n    },\n    \"level\": {\n      \"type\": \"integer\",\n      \"description\": \"Character level\",\n      \"example\": 70\n    },\n    \"experience\": {\n      \"type\": \"integer\",\n      \"description\": \"Character experience points\"\n    },\n    \"achievement_points\": {\n      \"type\": \"integer\",\n      \"description\": \"Total achievement points\",\n      \"example\": 15000\n    },\n    \"last_login_timestamp\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of last login\",\n      \"example\": 1718153645993\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-character-schema.json
tags: []
title: WoWCharacter
---
