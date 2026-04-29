---
description: A World of Warcraft guild
layout: schema
name: WoWGuild
properties_list:
- description: Guild ID
  name: id
  type: integer
- description: Guild name
  name: name
  type: string
- description: Guild faction
  name: faction
  type: object
- description: ''
  name: realm
  type: object
- description: Number of guild members
  name: member_count
  type: integer
- description: Guild achievement points
  name: achievement_points
  type: integer
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-guild-schema.json
slug: activision-blizzard-wo-w-guild
source_filename: activision-blizzard-wo-w-guild-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-guild-schema.json\",\n  \"title\": \"WoWGuild\",\n  \"description\": \"A World of Warcraft guild\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Guild ID\",\n      \"example\": 789012\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Guild name\",\n      \"example\": \"The Exodar\"\n    },\n    \"faction\": {\n      \"type\": \"object\",\n      \"description\": \"Guild faction\"\n    },\n    \"realm\": {\n      \"$ref\": \"#/components/schemas/WoWRealm\"\n    },\n    \"member_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of guild members\",\n      \"example\": 150\n    },\n    \"achievement_points\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Guild achievement points\",\n      \"example\": 5000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-guild-schema.json
tags: []
title: WoWGuild
---
