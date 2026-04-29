---
description: A StarCraft II profile
layout: schema
name: SC2Profile
properties_list:
- description: Profile summary
  name: summary
  type: object
- description: Profile snapshot data
  name: snapshot
  type: object
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-sc2-profile-schema.json
slug: activision-blizzard-sc2-profile
source_filename: activision-blizzard-sc2-profile-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-sc2-profile-schema.json\",\n  \"title\": \"SC2Profile\",\n  \"description\": \"A StarCraft II profile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"summary\": {\n      \"type\": \"object\",\n      \"description\": \"Profile summary\"\n    },\n    \"snapshot\": {\n      \"type\": \"object\",\n      \"description\": \"Profile snapshot data\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-sc2-profile-schema.json
tags: []
title: SC2Profile
---
