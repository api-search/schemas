---
description: Describes the content of the lexicon.
layout: schema
name: LexiconDescription
properties_list:
- description: ''
  name: Name
  type: object
- description: ''
  name: Attributes
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-lexicon-description-schema.json
slug: amazon-polly-lexicon-description
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-lexicon-description-schema.json\",\n  \"title\": \"LexiconDescription\",\n  \"description\": \"Describes the content of the lexicon.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconName\"\n        },\n        {\n          \"description\": \"Name of the lexicon.\"\n        }\n      ]\n    },\n    \"Attributes\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconAttributes\"\n        },\n        {\n          \"description\": \"Provides lexicon metadata.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-lexicon-description-schema.json
tags:
- AI
- AWS
- Machine Learning
- Speech Synthesis
- Text-To-Speech
- TTS
- Voice
- SSML
- Neural Engine
- Generative AI
title: LexiconDescription
---
