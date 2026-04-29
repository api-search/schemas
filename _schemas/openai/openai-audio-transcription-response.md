---
description: ''
layout: schema
name: TranscriptionResponse
properties_list:
- description: The transcribed text.
  name: text
  type: string
- description: The task performed, always transcribe.
  name: task
  type: string
- description: The detected or specified language of the audio.
  name: language
  type: string
- description: The duration of the input audio in seconds.
  name: duration
  type: number
- description: Extracted words and their corresponding timestamps. Only present when timestamp_granularities includes word.
  name: words
  type: array
- description: Segments of the transcribed text and their corresponding details. Only present when timestamp_granularities includes segment or response_format is verbose_json.
  name: segments
  type: array
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-audio-transcription-response-schema.json
slug: openai-audio-transcription-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"TranscriptionResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"text\": {\n      \"type\": \"string\",\n      \"description\": \"The transcribed text.\"\n    },\n    \"task\": {\n      \"type\": \"string\",\n      \"description\": \"The task performed, always transcribe.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The detected or specified language of the audio.\"\n    },\n    \"duration\": {\n      \"type\": \"number\",\n      \"description\": \"The duration of the input audio in seconds.\"\n    },\n    \"words\": {\n      \"type\": \"array\",\n      \"description\": \"Extracted words and their corresponding timestamps. Only present when timestamp_granularities includes word.\"\n    },\n    \"segments\": {\n      \"type\": \"array\",\n      \"description\": \"Segments of the transcribed text and their corresponding details. Only present\
  \ when timestamp_granularities includes segment or response_format is verbose_json.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-audio-transcription-response-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: TranscriptionResponse
---
