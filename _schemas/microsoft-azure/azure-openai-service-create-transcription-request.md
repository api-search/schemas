---
description: Request body for creating an audio transcription.
layout: schema
name: CreateTranscriptionRequest
properties_list:
- description: 'The audio file object to transcribe, in one of these formats: flac, mp3, mp4, mpeg, mpga, m4a, ogg, wav, or webm.'
  name: file
  type: string
- description: The language of the input audio. Supplying the input language in ISO-639-1 format will improve accuracy and latency.
  name: language
  type: string
- description: An optional text to guide the model's style or continue a previous audio segment.
  name: prompt
  type: string
- description: The format of the transcript output.
  name: response_format
  type: string
- description: The sampling temperature, between 0 and 1.
  name: temperature
  type: number
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-openai-service-create-transcription-request-schema.json
slug: azure-openai-service-create-transcription-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateTranscriptionRequest\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating an audio transcription.\",\n  \"properties\": {\n    \"file\": {\n      \"type\": \"string\",\n      \"description\": \"The audio file object to transcribe, in one of these formats: flac, mp3, mp4, mpeg, mpga, m4a, ogg, wav, or webm.\"\n    },\n    \"language\": {\n      \"type\": \"string\",\n      \"description\": \"The language of the input audio. Supplying the input language in ISO-639-1 format will improve accuracy and latency.\"\n    },\n    \"prompt\": {\n      \"type\": \"string\",\n      \"description\": \"An optional text to guide the model's style or continue a previous audio segment.\"\n    },\n    \"response_format\": {\n      \"type\": \"string\",\n      \"description\": \"The format of the transcript output.\"\n    },\n    \"temperature\": {\n      \"type\": \"number\",\n   \
  \   \"description\": \"The sampling temperature, between 0 and 1.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-openai-service-create-transcription-request-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: CreateTranscriptionRequest
---
