---
description: GetSpeechSynthesisTaskOutput schema from Amazon Polly API
layout: schema
name: GetSpeechSynthesisTaskOutput
properties_list:
- description: ''
  name: SynthesisTask
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-get-speech-synthesis-task-output-schema.json
slug: amazon-polly-get-speech-synthesis-task-output
source_filename: amazon-polly-get-speech-synthesis-task-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-get-speech-synthesis-task-output-schema.json\",\n  \"title\": \"GetSpeechSynthesisTaskOutput\",\n  \"description\": \"GetSpeechSynthesisTaskOutput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"SynthesisTask\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SynthesisTask\"\n        },\n        {\n          \"description\": \"SynthesisTask object that provides information from the requested task, including output format, creation time, task status, and so on.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-get-speech-synthesis-task-output-schema.json
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
title: GetSpeechSynthesisTaskOutput
---
