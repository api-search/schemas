---
description: A World of Warcraft realm
layout: schema
name: WoWRealm
properties_list:
- description: Realm ID
  name: id
  type: integer
- description: Realm name
  name: name
  type: string
- description: Realm slug
  name: slug
  type: string
- description: Region reference
  name: region
  type: object
- description: Realm category
  name: category
  type: string
- description: Realm locale
  name: locale
  type: string
- description: Realm timezone
  name: timezone
  type: string
- description: Realm type (Normal, RP, etc.)
  name: type
  type: object
- description: Whether this is a tournament realm
  name: is_tournament
  type: boolean
provider_name: activision-blizzard
provider_slug: activision-blizzard
schema_file: json-schema/activision-blizzard-wo-w-realm-schema.json
slug: activision-blizzard-wo-w-realm
source_filename: activision-blizzard-wo-w-realm-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-realm-schema.json\",\n  \"title\": \"WoWRealm\",\n  \"description\": \"A World of Warcraft realm\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Realm ID\",\n      \"example\": 1\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Realm name\",\n      \"example\": \"Area 52\"\n    },\n    \"slug\": {\n      \"type\": \"string\",\n      \"description\": \"Realm slug\",\n      \"example\": \"area-52\"\n    },\n    \"region\": {\n      \"type\": \"object\",\n      \"description\": \"Region reference\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Realm category\",\n      \"example\": \"United States\"\n    },\n    \"locale\": {\n      \"type\"\
  : \"string\",\n      \"description\": \"Realm locale\",\n      \"example\": \"en_US\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Realm timezone\",\n      \"example\": \"America/New_York\"\n    },\n    \"type\": {\n      \"type\": \"object\",\n      \"description\": \"Realm type (Normal, RP, etc.)\"\n    },\n    \"is_tournament\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is a tournament realm\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/activision-blizzard/refs/heads/main/json-schema/activision-blizzard-wo-w-realm-schema.json
tags: []
title: WoWRealm
---
