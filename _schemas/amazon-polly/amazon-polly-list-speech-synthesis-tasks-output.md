---
description: ListSpeechSynthesisTasksOutput schema from Amazon Polly API
layout: schema
name: ListSpeechSynthesisTasksOutput
properties_list:
- description: ''
  name: NextToken
  type: object
- description: ''
  name: SynthesisTasks
  type: object
provider_name: Amazon Polly
provider_slug: amazon-polly
schema_file: json-schema/amazon-polly-list-speech-synthesis-tasks-output-schema.json
slug: amazon-polly-list-speech-synthesis-tasks-output
source_filename: amazon-polly-list-speech-synthesis-tasks-output-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-list-speech-synthesis-tasks-output-schema.json\",\n  \"title\": \"ListSpeechSynthesisTasksOutput\",\n  \"description\": \"ListSpeechSynthesisTasksOutput schema from Amazon Polly API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"NextToken\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/NextToken\"\n        },\n        {\n          \"description\": \"An opaque pagination token returned from the previous List operation in this request. If present, this indicates where to continue the listing.\"\n        }\n      ]\n    },\n    \"SynthesisTasks\": {\n      \"allOf\": [\n        {\n          \"$ref\": \"#/components/schemas/SynthesisTasks\"\n        },\n        {\n          \"description\": \"List of SynthesisTask objects that provides information from the\
  \ specified task in the list request, including output format, creation time, task status, and so on.\"\n        }\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/amazon-polly/refs/heads/main/json-schema/amazon-polly-list-speech-synthesis-tasks-output-schema.json
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
title: ListSpeechSynthesisTasksOutput
---
