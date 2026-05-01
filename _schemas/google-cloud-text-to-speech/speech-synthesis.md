---
description: Schema for a Google Cloud Text-to-Speech synthesis request.
layout: schema
name: Speech Synthesis Request
properties_list:
- description: The input to be synthesized.
  name: input
  type: object
- description: The desired voice configuration.
  name: voice
  type: object
- description: Audio configuration for the synthesized output.
  name: audioConfig
  type: object
provider_name: Google Cloud Text-To-Speech
provider_slug: google-cloud-text-to-speech
schema_file: json-schema/speech-synthesis.json
slug: speech-synthesis
source_filename: speech-synthesis.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-cloud-text-to-speech/refs/heads/main/json-schema/speech-synthesis.json\",\n  \"title\": \"Speech Synthesis Request\",\n  \"description\": \"Schema for a Google Cloud Text-to-Speech synthesis request.\",\n  \"type\": \"object\",\n  \"required\": [\"input\", \"voice\", \"audioConfig\"],\n  \"properties\": {\n    \"input\": {\n      \"type\": \"object\",\n      \"description\": \"The input to be synthesized.\",\n      \"properties\": {\n        \"text\": {\n          \"type\": \"string\",\n          \"description\": \"Raw text to be synthesized.\"\n        },\n        \"ssml\": {\n          \"type\": \"string\",\n          \"description\": \"SSML markup to be synthesized.\"\n        }\n      }\n    },\n    \"voice\": {\n      \"type\": \"object\",\n      \"description\": \"The desired voice configuration.\",\n      \"required\": [\"languageCode\"\
  ],\n      \"properties\": {\n        \"languageCode\": {\n          \"type\": \"string\",\n          \"description\": \"BCP-47 language tag.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Name of the voice.\"\n        },\n        \"ssmlGender\": {\n          \"type\": \"string\",\n          \"enum\": [\"SSML_VOICE_GENDER_UNSPECIFIED\", \"MALE\", \"FEMALE\", \"NEUTRAL\"],\n          \"description\": \"Preferred gender of the voice.\"\n        }\n      }\n    },\n    \"audioConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Audio configuration for the synthesized output.\",\n      \"required\": [\"audioEncoding\"],\n      \"properties\": {\n        \"audioEncoding\": {\n          \"type\": \"string\",\n          \"enum\": [\"AUDIO_ENCODING_UNSPECIFIED\", \"LINEAR16\", \"MP3\", \"OGG_OPUS\", \"MULAW\", \"ALAW\"],\n          \"description\": \"The encoding format of the output audio.\"\n        },\n        \"speakingRate\"\
  : {\n          \"type\": \"number\",\n          \"description\": \"Speaking rate, range [0.25, 4.0].\"\n        },\n        \"pitch\": {\n          \"type\": \"number\",\n          \"description\": \"Pitch adjustment, range [-20.0, 20.0].\"\n        },\n        \"volumeGainDb\": {\n          \"type\": \"number\",\n          \"description\": \"Volume gain in dB, range [-96.0, 16.0].\"\n        },\n        \"sampleRateHertz\": {\n          \"type\": \"integer\",\n          \"description\": \"Sample rate in Hz for the output audio.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-cloud-text-to-speech/refs/heads/main/json-schema/speech-synthesis.json
tags:
- Audio
- Google Cloud
- Machine Learning
- Speech Synthesis
- Text-To-Speech
title: Speech Synthesis Request
---
