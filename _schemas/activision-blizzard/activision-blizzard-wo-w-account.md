---
description: A World of Warcraft account
layout: schema
name: WoWAccount
properties_list:
- description: Account ID
  name: id
  type: integer
- description: List of characters on this account
  name: characters
  type: array
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-account-schema.json
slug: activision-blizzard-wo-w-account
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-account-schema.json\",\n  \"title\": \"WoWAccount\",\n  \"description\": \"A World of Warcraft account\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Account ID\",\n      \"example\": 1\n    },\n    \"characters\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/WoWCharacterSummary\"\n      },\n      \"description\": \"List of characters on this account\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-account-schema.json
tags: []
title: WoWAccount
---
