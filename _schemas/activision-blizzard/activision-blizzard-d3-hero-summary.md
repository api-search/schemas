---
description: Summary of a Diablo III hero
layout: schema
name: D3HeroSummary
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
- description: Hero level
  name: level
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
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-d3-hero-summary-schema.json
slug: activision-blizzard-d3-hero-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-d3-hero-summary-schema.json\",\n  \"title\": \"D3HeroSummary\",\n  \"description\": \"Summary of a Diablo III hero\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Hero ID\",\n      \"example\": 12345\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Hero name\",\n      \"example\": \"Zul'jin\"\n    },\n    \"class\": {\n      \"type\": \"string\",\n      \"description\": \"Hero class\",\n      \"example\": \"barbarian\"\n    },\n    \"level\": {\n      \"type\": \"integer\",\n      \"description\": \"Hero level\",\n      \"example\": 70\n    },\n    \"hardcore\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a hardcore hero\"\n    },\n    \"seasonal\"\
  : {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a seasonal hero\"\n    },\n    \"dead\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this hero is dead\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-d3-hero-summary-schema.json
tags: []
title: D3HeroSummary
---
