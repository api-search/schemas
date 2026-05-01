---
description: Schema for a Google Cloud Translation text translation request.
layout: schema
name: Translation Request
properties_list:
- description: The content of the input text to translate.
  name: contents
  type: array
- description: The format of the source text, e.g., text/plain or text/html.
  name: mimeType
  type: string
- description: BCP-47 language code of the input text.
  name: sourceLanguageCode
  type: string
- description: BCP-47 language code of the target translation language.
  name: targetLanguageCode
  type: string
- description: Optional glossary to use for translation.
  name: glossaryConfig
  type: object
- description: The model resource name to use for translation.
  name: model
  type: string
provider_name: Google Cloud Translation
provider_slug: google-cloud-translation
schema_file: json-schema/translation.json
slug: translation
source_filename: translation.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-translation/refs/heads/main/json-schema/translation.json\",\n  \"title\": \"Translation Request\",\n  \"description\": \"Schema for a Google Cloud Translation text translation request.\",\n  \"type\": \"object\",\n  \"required\": [\"contents\", \"targetLanguageCode\"],\n  \"properties\": {\n    \"contents\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"The content of the input text to translate.\"\n    },\n    \"mimeType\": {\n      \"type\": \"string\",\n      \"description\": \"The format of the source text, e.g., text/plain or text/html.\"\n    },\n    \"sourceLanguageCode\": {\n      \"type\": \"string\",\n      \"description\": \"BCP-47 language code of the input text.\"\n    },\n    \"targetLanguageCode\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"BCP-47 language code of the target translation language.\"\n    },\n    \"glossaryConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Optional glossary to use for translation.\",\n      \"properties\": {\n        \"glossary\": {\n          \"type\": \"string\",\n          \"description\": \"Resource name of the glossary.\"\n        },\n        \"ignoreCase\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether to ignore case when matching glossary terms.\"\n        }\n      }\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The model resource name to use for translation.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-translation/refs/heads/main/json-schema/translation.json
tags:
- Google Cloud
- Language
- Localization
- Machine Learning
- Translation
title: Translation Request
---
