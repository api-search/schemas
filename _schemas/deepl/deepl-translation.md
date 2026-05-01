---
description: A translation result returned by the DeepL /translate endpoint.
layout: schema
name: DeepL Translation
properties_list:
- description: ''
  name: translations
  type: array
provider_name: DeepL
provider_slug: deepl
schema_file: json-schema/deepl-translation.json
slug: deepl-translation
source_filename: deepl-translation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api-evangelist.github.io/deepl/json-schema/deepl-translation.json\",\n  \"title\": \"DeepL Translation\",\n  \"description\": \"A translation result returned by the DeepL /translate endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"translations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"detected_source_language\": {\"type\": \"string\"},\n          \"text\": {\"type\": \"string\"}\n        },\n        \"required\": [\"text\"]\n      }\n    }\n  },\n  \"required\": [\"translations\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/deepl/refs/heads/main/json-schema/deepl-translation.json
tags:
- Artificial Intelligence
- Deep Learning
- Glossaries
- Localization
- Machine Learning
- Machine Translation
- Translation
title: DeepL Translation
---
