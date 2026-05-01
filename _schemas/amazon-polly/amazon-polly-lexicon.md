---
description: Provides lexicon name and lexicon content in string format. For more information, see <a href="https://www.w3.org/TR/pronunciation-lexicon/">Pronunciation Lexicon Specification (PLS) Version 1.0</a>.
layout: schema
name: Lexicon
properties_list:
- description: ''
  name: Content
  type: object
- description: ''
  name: Name
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-lexicon-schema.json
slug: amazon-polly-lexicon
source_filename: amazon-polly-lexicon-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-lexicon-schema.json\",\n  \"title\": \"Lexicon\",\n  \"description\": \"Provides lexicon name and lexicon content in string format. For more information, see <a href=\\\"https://www.w3.org/TR/pronunciation-lexicon/\\\">Pronunciation Lexicon Specification (PLS) Version 1.0</a>.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconContent\"\n        },\n        {\n          \"description\": \"Lexicon content in string format. The content of a lexicon must be in PLS format.\"\n        }\n      ]\n    },\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconName\"\n        },\n        {\n          \"description\": \"Name of the lexicon.\"\n        }\n    \
  \  ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-lexicon-schema.json
tags:
- AI
- Machine Learning
- Speech Synthesis
- Text-To-Speech
- TTS
- Voice
- SSML
- Neural Engine
- Generative AI
title: Lexicon
---
