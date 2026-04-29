---
description: ''
layout: schema
name: CreateTranslationRequest
properties_list:
- description: 'The audio file to translate, in one of these formats: flac, mp3, mp4, mpeg, mpga, m4a, ogg, wav, or webm. File uploads are limited to 25 MB.'
  name: file
  type: string
- description: ID of the model to use. Only whisper-1 is currently available for translation.
  name: model
  type: string
- description: An optional text to guide the model's style or continue a previous audio segment. The prompt should be in English.
  name: prompt
  type: string
- description: The format of the transcript output. Defaults to json.
  name: response_format
  type: string
- description: The sampling temperature, between 0 and 1.
  name: temperature
  type: number
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-audio-create-translation-request-schema.json
slug: openai-audio-create-translation-request
source_filename: openai-audio-create-translation-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTranslationRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"file\": {\n      \"type\": \"string\",\n      \"description\": \"The audio file to translate, in one of these formats: flac, mp3, mp4, mpeg, mpga, m4a, ogg, wav, or webm. File uploads are limited to 25 MB.\"\n    },\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the model to use. Only whisper-1 is currently available for translation.\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"An optional text to guide the model's style or continue a previous audio segment. The prompt should be in English.\"\n    },\n    \"response_format\": {\n      \"type\": \"string\",\n      \"description\": \"The format of the transcript output. Defaults to json.\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n      \"description\": \"The sampling temperature,\
  \ between 0 and 1.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-audio-create-translation-request-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: CreateTranslationRequest
---
