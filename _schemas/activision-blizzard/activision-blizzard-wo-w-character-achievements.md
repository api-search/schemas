---
description: Character achievements summary
layout: schema
name: WoWCharacterAchievements
properties_list:
- description: Total achievements completed
  name: total_quantity
  type: integer
- description: Total achievement points
  name: total_points
  type: integer
- description: List of completed achievements
  name: achievements
  type: array
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-character-achievements-schema.json
slug: activision-blizzard-wo-w-character-achievements
source_filename: activision-blizzard-wo-w-character-achievements-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-character-achievements-schema.json\",\n  \"title\": \"WoWCharacterAchievements\",\n  \"description\": \"Character achievements summary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total_quantity\": {\n      \"type\": \"integer\",\n      \"description\": \"Total achievements completed\",\n      \"example\": 2500\n    },\n    \"total_points\": {\n      \"type\": \"integer\",\n      \"description\": \"Total achievement points\",\n      \"example\": 15000\n    },\n    \"achievements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      },\n      \"description\": \"List of completed achievements\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-character-achievements-schema.json
tags: []
title: WoWCharacterAchievements
---
