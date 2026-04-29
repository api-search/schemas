---
description: PutLexiconInput schema from Amazon Polly API
layout: schema
name: PutLexiconInput
properties_list:
- description: ''
  name: Content
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-put-lexicon-input-schema.json
slug: amazon-polly-put-lexicon-input
source_filename: amazon-polly-put-lexicon-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-put-lexicon-input-schema.json\",\n  \"title\": \"PutLexiconInput\",\n  \"description\": \"PutLexiconInput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"Content\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/LexiconContent\"\n        },\n        {\n          \"description\": \"Content of the PLS lexicon as string data.\"\n        }\n      ]\n    }\n  },\n  \"required\": [\n    \"Content\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-put-lexicon-input-schema.json
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
title: PutLexiconInput
---
