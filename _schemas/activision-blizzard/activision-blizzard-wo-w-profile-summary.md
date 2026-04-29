---
description: World of Warcraft account profile summary
layout: schema
name: WoWProfileSummary
properties_list:
- description: Account ID
  name: id
  type: integer
- description: WoW accounts linked to the Battle.net account
  name: wow_accounts
  type: array
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-profile-summary-schema.json
slug: activision-blizzard-wo-w-profile-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-profile-summary-schema.json\",\n  \"title\": \"WoWProfileSummary\",\n  \"description\": \"World of Warcraft account profile summary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Account ID\",\n      \"example\": 12345678\n    },\n    \"wow_accounts\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/WoWAccount\"\n      },\n      \"description\": \"WoW accounts linked to the Battle.net account\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-profile-summary-schema.json
tags: []
title: WoWProfileSummary
---
