---
description: Summary of a WoW character
layout: schema
name: WoWCharacterSummary
properties_list:
- description: Character reference with href
  name: character
  type: object
- description: Protected character reference
  name: protected_character
  type: object
- description: Character name
  name: name
  type: string
- description: Character ID
  name: id
  type: integer
- description: ''
  name: realm
  type: object
- description: Playable class reference
  name: playable_class
  type: object
- description: Playable race reference
  name: playable_race
  type: object
- description: Character gender
  name: gender
  type: object
- description: Character faction (Alliance or Horde)
  name: faction
  type: object
- description: Character level
  name: level
  type: integer
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-character-summary-schema.json
slug: activision-blizzard-wo-w-character-summary
source_filename: activision-blizzard-wo-w-character-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-character-summary-schema.json\",\n  \"title\": \"WoWCharacterSummary\",\n  \"description\": \"Summary of a WoW character\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"character\": {\n      \"type\": \"object\",\n      \"description\": \"Character reference with href\"\n    },\n    \"protected_character\": {\n      \"type\": \"object\",\n      \"description\": \"Protected character reference\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Character name\",\n      \"example\": \"Thrall\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Character ID\",\n      \"example\": 123456\n    },\n    \"realm\": {\n      \"$ref\": \"#/components/schemas/WoWRealm\"\n    },\n    \"playable_class\": {\n      \"type\"\
  : \"object\",\n      \"description\": \"Playable class reference\"\n    },\n    \"playable_race\": {\n      \"type\": \"object\",\n      \"description\": \"Playable race reference\"\n    },\n    \"gender\": {\n      \"type\": \"object\",\n      \"description\": \"Character gender\"\n    },\n    \"faction\": {\n      \"type\": \"object\",\n      \"description\": \"Character faction (Alliance or Horde)\"\n    },\n    \"level\": {\n      \"type\": \"integer\",\n      \"description\": \"Character level\",\n      \"example\": 70\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-character-summary-schema.json
tags: []
title: WoWCharacterSummary
---
