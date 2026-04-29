---
description: SynthesizeSpeechOutput schema from Amazon Polly API
layout: schema
name: SynthesizeSpeechOutput
properties_list:
- description: ''
  name: AudioStream
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-synthesize-speech-output-schema.json
slug: amazon-polly-synthesize-speech-output
source_filename: amazon-polly-synthesize-speech-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-synthesize-speech-output-schema.json\",\n  \"title\": \"SynthesizeSpeechOutput\",\n  \"description\": \"SynthesizeSpeechOutput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"AudioStream\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/AudioStream\"\n        },\n        {\n          \"description\": \" Stream containing the synthesized speech. \"\n        }\n      ]\n    }\n  },\n  \"example\": {\n    \"AudioStream\": \"TEXT\",\n    \"ContentType\": \"audio/mpeg\",\n    \"RequestCharacters\": 37\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-synthesize-speech-output-schema.json
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
title: SynthesizeSpeechOutput
---
