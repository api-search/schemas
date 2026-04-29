---
description: Index of WoW realms
layout: schema
name: WoWRealmsIndex
properties_list:
- description: List of realms
  name: realms
  type: array
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-realms-index-schema.json
slug: activision-blizzard-wo-w-realms-index
source_filename: activision-blizzard-wo-w-realms-index-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-realms-index-schema.json\",\n  \"title\": \"WoWRealmsIndex\",\n  \"description\": \"Index of WoW realms\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"realms\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/WoWRealm\"\n      },\n      \"description\": \"List of realms\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-realms-index-schema.json
tags: []
title: WoWRealmsIndex
---
