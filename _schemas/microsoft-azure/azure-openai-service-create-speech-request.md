---
description: Request body for generating speech from text.
layout: schema
name: CreateSpeechRequest
properties_list:
- description: The TTS model to use.
  name: model
  type: string
- description: The text to generate audio for.
  name: input
  type: string
- description: The voice to use when generating the audio.
  name: voice
  type: string
- description: The format to audio in.
  name: response_format
  type: string
- description: The speed of the generated audio.
  name: speed
  type: number
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-create-speech-request-schema.json
slug: azure-openai-service-create-speech-request
source_filename: azure-openai-service-create-speech-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateSpeechRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for generating speech from text.\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"The TTS model to use.\"\n    },\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"The text to generate audio for.\"\n    },\n    \"voice\": {\n      \"type\": \"string\",\n      \"description\": \"The voice to use when generating the audio.\"\n    },\n    \"response_format\": {\n      \"type\": \"string\",\n      \"description\": \"The format to audio in.\"\n    },\n    \"speed\": {\n      \"type\": \"number\",\n      \"description\": \"The speed of the generated audio.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-create-speech-request-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CreateSpeechRequest
---
