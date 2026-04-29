---
description: ''
layout: schema
name: CreateSpeechRequest
properties_list:
- description: One of the available TTS models. tts-1 is optimized for speed, tts-1-hd is optimized for quality, and gpt-4o-mini-tts supports advanced voice instructions.
  name: model
  type: string
- description: The text to generate audio for. The maximum length is 4096 characters.
  name: input
  type: string
- description: The voice to use when generating the audio. Previews of the voices are available in the Text to Speech guide.
  name: voice
  type: string
- description: Control the voice of your generated audio with additional instructions. Only supported with gpt-4o-mini-tts.
  name: instructions
  type: string
- description: The format to audio in. Supported formats are mp3, opus, aac, flac, wav, and pcm. Opus is recommended for internet streaming and communication, aac for digital audio compression, and flac for lossless
  name: response_format
  type: string
- description: The speed of the generated audio. Select a value from 0.25 to 4.0. 1.0 is the default.
  name: speed
  type: number
provider_name: OpenAI
provider_slug: openai
schema_file: json-schema/openai-audio-create-speech-request-schema.json
slug: openai-audio-create-speech-request
source_filename: openai-audio-create-speech-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateSpeechRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"model\": {\n      \"type\": \"string\",\n      \"description\": \"One of the available TTS models. tts-1 is optimized for speed, tts-1-hd is optimized for quality, and gpt-4o-mini-tts supports advanced voice instructions.\"\n    },\n    \"input\": {\n      \"type\": \"string\",\n      \"description\": \"The text to generate audio for. The maximum length is 4096 characters.\"\n    },\n    \"voice\": {\n      \"type\": \"string\",\n      \"description\": \"The voice to use when generating the audio. Previews of the voices are available in the Text to Speech guide.\"\n    },\n    \"instructions\": {\n      \"type\": \"string\",\n      \"description\": \"Control the voice of your generated audio with additional instructions. Only supported with gpt-4o-mini-tts.\"\n    },\n    \"response_format\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The format to audio in. Supported formats are mp3, opus, aac, flac, wav, and pcm. Opus is recommended for internet streaming and communication, aac for digital audio compression, and flac for lossless audio compression.\"\n    },\n    \"speed\": {\n      \"type\": \"number\",\n      \"description\": \"The speed of the generated audio. Select a value from 0.25 to 4.0. 1.0 is the default.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openai/refs/heads/main/json-schema/openai-audio-create-speech-request-schema.json
tags:
- AI
- Artificial Intelligence
- Large Language Models
- T1
title: CreateSpeechRequest
---
