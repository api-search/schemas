---
description: ''
layout: schema
name: Phrase
properties_list:
- description: Phrase category (e.g., Greetings, Dining, Transportation)
  name: category
  type: string
- description: Phrase in source language
  name: original
  type: string
- description: Phrase in destination language
  name: translation
  type: string
- description: Phonetic pronunciation guide
  name: phonetic
  type: string
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/phrase.json
slug: phrase
source_filename: phrase.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/phrase.json\",\n  \"title\": \"Phrase\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Phrase category (e.g., Greetings, Dining, Transportation)\"\n    },\n    \"original\": {\n      \"type\": \"string\",\n      \"description\": \"Phrase in source language\"\n    },\n    \"translation\": {\n      \"type\": \"string\",\n      \"description\": \"Phrase in destination language\"\n    },\n    \"phonetic\": {\n      \"type\": \"string\",\n      \"description\": \"Phonetic pronunciation guide\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/phrase.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: Phrase
---
