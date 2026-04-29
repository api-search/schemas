---
description: ''
layout: schema
name: TranslationResponse
properties_list:
- description: The translated text in English.
  name: text
  type: string
- description: The task performed, always translate.
  name: task
  type: string
- description: The detected language of the input audio.
  name: language
  type: string
- description: The duration of the input audio in seconds.
  name: duration
  type: number
- description: Segments of the translated text with timestamps.
  name: segments
  type: array
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-audio-translation-response-schema.json
slug: openai-audio-translation-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TranslationResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The translated text in English.\"\n    },\n    \"task\": {\n      \"type\": \"string\",\n      \"description\": \"The task performed, always translate.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The detected language of the input audio.\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"The duration of the input audio in seconds.\"\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Segments of the translated text with timestamps.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-audio-translation-response-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: TranslationResponse
---
