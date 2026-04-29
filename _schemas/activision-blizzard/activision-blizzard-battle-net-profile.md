---
description: Battle.net account profile
layout: schema
name: BattleNetProfile
properties_list:
- description: Account ID
  name: id
  type: integer
- description: Battle.net BattleTag
  name: battletag
  type: string
- description: OAuth2 subject identifier
  name: sub
  type: string
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-battle-net-profile-schema.json
slug: activision-blizzard-battle-net-profile
source_filename: activision-blizzard-battle-net-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-battle-net-profile-schema.json\",\n  \"title\": \"BattleNetProfile\",\n  \"description\": \"Battle.net account profile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Account ID\",\n      \"example\": 12345678\n    },\n    \"battletag\": {\n      \"type\": \"string\",\n      \"description\": \"Battle.net BattleTag\",\n      \"example\": \"Player#1234\"\n    },\n    \"sub\": {\n      \"type\": \"string\",\n      \"description\": \"OAuth2 subject identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-battle-net-profile-schema.json
tags: []
title: BattleNetProfile
---
