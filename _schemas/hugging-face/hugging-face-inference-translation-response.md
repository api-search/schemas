---
description: ''
layout: schema
name: TranslationResponse
properties_list:
- description: The translated text
  name: translation_text
  type: string
provider_name: Hugging Face
provider_slug: hugging-face
schema_file: json-schema/hugging-face-inference-translation-response-schema.json
slug: hugging-face-inference-translation-response
source_filename: hugging-face-inference-translation-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TranslationResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"translation_text\": {\n      \"type\": \"string\",\n      \"description\": \"The translated text\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hugging-face/refs/heads/main/json-schema/hugging-face-inference-translation-response-schema.json
tags: []
title: TranslationResponse
---
