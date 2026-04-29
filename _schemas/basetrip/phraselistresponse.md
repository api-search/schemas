---
description: ''
layout: schema
name: PhraseListResponse
properties_list:
- description: Destination language code
  name: language
  type: string
- description: ''
  name: phrases
  type: array
provider_name: Basetrip
provider_slug: basetrip
schema_file: json-schema/phraselistresponse.json
slug: phraselistresponse
source_filename: phraselistresponse.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/phraselistresponse.json\",\n  \"title\": \"PhraseListResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"Destination language code\"\n    },\n    \"phrases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Phrase\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/basetrip/refs/heads/main/json-schema/phraselistresponse.json
tags:
- Cities
- Countries
- Health
- Safety
- Travel
- Visa
title: PhraseListResponse
---
