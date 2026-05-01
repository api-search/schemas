---
description: JSON Schema for the Google Cloud Translation API request and response objects.
layout: schema
name: Google Cloud Translation API Schema
properties_list: []
provider_name: Google Cloud Translation API
provider_slug: google-translate
schema_file: json-schema/google-translate.json
slug: google-translate
source_filename: google-translate.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-translate/refs/heads/main/json-schema/google-translate.json\",\n  \"title\": \"Google Cloud Translation API Schema\",\n  \"description\": \"JSON Schema for the Google Cloud Translation API request and response objects.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"TranslateTextRequest\": {\n      \"type\": \"object\",\n      \"required\": [\"q\", \"target\"],\n      \"properties\": {\n        \"q\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The text to translate. Specify up to 128 strings.\"\n        },\n        \"target\": {\n          \"type\": \"string\",\n          \"description\": \"The target language code (ISO 639-1).\"\n        },\n        \"source\": {\n          \"type\": \"string\",\n          \"description\": \"The source language\
  \ code (ISO 639-1).\"\n        },\n        \"format\": {\n          \"type\": \"string\",\n          \"enum\": [\"text\", \"html\"],\n          \"description\": \"The format of the source text.\"\n        },\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"The translation model (base or nmt).\"\n        }\n      }\n    },\n    \"TranslateTextResponse\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"data\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"translations\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"$ref\": \"#/$defs/Translation\"\n              }\n            }\n          }\n        }\n      }\n    },\n    \"Translation\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"translatedText\": {\n          \"type\": \"string\",\n          \"description\": \"The translated text.\"\n        },\n        \"detectedSourceLanguage\": {\n\
  \          \"type\": \"string\",\n          \"description\": \"The detected source language code.\"\n        },\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"The translation model used.\"\n        }\n      }\n    },\n    \"DetectLanguageRequest\": {\n      \"type\": \"object\",\n      \"required\": [\"q\"],\n      \"properties\": {\n        \"q\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"The text to detect the language of.\"\n        }\n      }\n    },\n    \"Detection\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"The detected language code.\"\n        },\n        \"confidence\": {\n          \"type\": \"number\",\n          \"description\": \"Confidence level of the detection.\"\n        },\n        \"isReliable\": {\n          \"type\": \"boolean\",\n \
  \         \"description\": \"Whether the detection is reliable.\"\n        }\n      }\n    },\n    \"Language\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"language\": {\n          \"type\": \"string\",\n          \"description\": \"The language code (ISO 639-1).\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Human-readable language name.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-translate/refs/heads/main/json-schema/google-translate.json
tags:
- Google Cloud
- Internationalization
- Language Detection
- Localization
- Machine Translation
- Natural Language Processing
- Translation
title: Google Cloud Translation API Schema
---
