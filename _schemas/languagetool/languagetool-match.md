---
description: A single grammar or style match returned by the LanguageTool /check endpoint.
layout: schema
name: LanguageTool Match
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: shortMessage
  type: string
- description: ''
  name: offset
  type: integer
- description: ''
  name: length
  type: integer
- description: ''
  name: replacements
  type: array
- description: ''
  name: context
  type: object
- description: ''
  name: sentence
  type: string
- description: ''
  name: rule
  type: object
provider_name: LanguageTool
provider_slug: languagetool
schema_file: json-schema/languagetool-match-schema.json
slug: languagetool-match
source_filename: languagetool-match-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/languagetool/main/json-schema/languagetool-match-schema.json\",\n  \"title\": \"LanguageTool Match\",\n  \"description\": \"A single grammar or style match returned by the LanguageTool /check endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"message\": { \"type\": \"string\" },\n    \"shortMessage\": { \"type\": \"string\" },\n    \"offset\": { \"type\": \"integer\" },\n    \"length\": { \"type\": \"integer\" },\n    \"replacements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"value\": { \"type\": \"string\" }\n        }\n      }\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"text\": { \"type\": \"string\" },\n        \"offset\": { \"type\": \"integer\" },\n        \"length\": { \"type\": \"integer\" }\n   \
  \   }\n    },\n    \"sentence\": { \"type\": \"string\" },\n    \"rule\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": { \"type\": \"string\" },\n        \"description\": { \"type\": \"string\" },\n        \"issueType\": { \"type\": \"string\" },\n        \"category\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": { \"type\": \"string\" },\n            \"name\": { \"type\": \"string\" }\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\"message\", \"offset\", \"length\", \"rule\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/languagetool/refs/heads/main/json-schema/languagetool-match-schema.json
tags:
- Grammar
- Language
- Proofreading
- Spell Check
- Style Check
- Text Analysis
title: LanguageTool Match
---
