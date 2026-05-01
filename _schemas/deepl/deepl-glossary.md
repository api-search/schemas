---
description: A custom glossary used to enforce terminology in DeepL translations.
layout: schema
name: DeepL Glossary
properties_list:
- description: ''
  name: glossary_id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: ready
  type: boolean
- description: ''
  name: source_lang
  type: string
- description: ''
  name: target_lang
  type: string
- description: ''
  name: creation_time
  type: string
- description: ''
  name: entry_count
  type: integer
provider_name: DeepL
provider_slug: deepl
schema_file: json-schema/deepl-glossary.json
slug: deepl-glossary
source_filename: deepl-glossary.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/deepl/json-schema/deepl-glossary.json\",\n  \"title\": \"DeepL Glossary\",\n  \"description\": \"A custom glossary used to enforce terminology in DeepL translations.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"glossary_id\": {\"type\": \"string\"},\n    \"name\": {\"type\": \"string\"},\n    \"ready\": {\"type\": \"boolean\"},\n    \"source_lang\": {\"type\": \"string\"},\n    \"target_lang\": {\"type\": \"string\"},\n    \"creation_time\": {\"type\": \"string\", \"format\": \"date-time\"},\n    \"entry_count\": {\"type\": \"integer\"}\n  },\n  \"required\": [\"glossary_id\", \"name\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/deepl/refs/heads/main/json-schema/deepl-glossary.json
tags:
- Artificial Intelligence
- Deep Learning
- Glossaries
- Localization
- Machine Learning
- Machine Translation
- Translation
title: DeepL Glossary
---
