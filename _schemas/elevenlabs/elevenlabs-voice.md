---
description: Represents a voice in the ElevenLabs platform, including pre-built, cloned, and designed voices with their associated metadata, settings, and audio samples.
layout: schema
name: ElevenLabs Voice
properties_list:
- description: Unique identifier for the voice.
  name: voice_id
  type: string
- description: Display name of the voice.
  name: name
  type: string
- description: The category indicating how the voice was created.
  name: category
  type: string
- description: Human-readable description of the voice characteristics and intended use.
  name: description
  type: string
- description: Key-value labels describing voice characteristics such as accent, age, gender, and use case.
  name: labels
  type: object
- description: URL to a preview audio sample of the voice.
  name: preview_url
  type: string
- description: ''
  name: settings
  type: object
- description: Audio samples associated with the voice, used for cloning and preview.
  name: samples
  type: array
- description: Sharing and publication status of the voice.
  name: sharing
  type: object
- description: List of model identifiers that produce the best results with this voice.
  name: high_quality_base_model_ids
  type: array
provider_name: elevenlabs
provider_slug: elevenlabs
schema_file: json-schema/elevenlabs-voice-schema.json
slug: elevenlabs-voice
source_filename: elevenlabs-voice-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://elevenlabs.io/schemas/elevenlabs/voice.json\",\n  \"title\": \"ElevenLabs Voice\",\n  \"description\": \"Represents a voice in the ElevenLabs platform, including pre-built, cloned, and designed voices with their associated metadata, settings, and audio samples.\",\n  \"type\": \"object\",\n  \"required\": [\"voice_id\", \"name\"],\n  \"properties\": {\n    \"voice_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the voice.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the voice.\",\n      \"minLength\": 1,\n      \"maxLength\": 200\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category indicating how the voice was created.\",\n      \"enum\": [\"premade\", \"cloned\", \"designed\", \"professional\"]\n    },\n    \"description\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"Human-readable description of the voice characteristics and intended use.\"\n    },\n    \"labels\": {\n      \"type\": \"object\",\n      \"description\": \"Key-value labels describing voice characteristics such as accent, age, gender, and use case.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n    },\n    \"preview_url\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL to a preview audio sample of the voice.\"\n    },\n    \"settings\": {\n      \"$ref\": \"#/$defs/VoiceSettings\"\n    },\n    \"samples\": {\n      \"type\": \"array\",\n      \"description\": \"Audio samples associated with the voice, used for cloning and preview.\",\n      \"items\": {\n        \"$ref\": \"#/$defs/VoiceSample\"\n      }\n    },\n    \"sharing\": {\n      \"type\": \"object\",\n      \"description\": \"Sharing and publication status of the voice.\",\n      \"properties\": {\n        \"status\": {\n  \
  \        \"type\": \"string\",\n          \"description\": \"Whether the voice is shared publicly.\",\n          \"enum\": [\"enabled\", \"disabled\"]\n        },\n        \"public_owner_id\": {\n          \"type\": \"string\",\n          \"description\": \"Public identifier of the voice owner.\"\n        },\n        \"cloned_by_count\": {\n          \"type\": \"integer\",\n          \"description\": \"Number of users who have cloned or added this voice.\",\n          \"minimum\": 0\n        }\n      }\n    },\n    \"high_quality_base_model_ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of model identifiers that produce the best results with this voice.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$defs\": {\n    \"VoiceSettings\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration parameters that control the voice's speech synthesis characteristics.\",\n      \"properties\": {\n        \"stability\": {\n     \
  \     \"type\": \"number\",\n          \"description\": \"Controls the consistency of the voice output. Higher values produce more stable, predictable speech. Lower values introduce more variation.\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        },\n        \"similarity_boost\": {\n          \"type\": \"number\",\n          \"description\": \"Controls how closely the generated speech matches the original voice. Higher values increase fidelity to the target voice.\",\n          \"minimum\": 0,\n          \"maximum\": 1\n        },\n        \"style\": {\n          \"type\": \"number\",\n          \"description\": \"Controls the expressiveness and stylistic variation of the speech delivery.\",\n          \"minimum\": 0,\n          \"maximum\": 1,\n          \"default\": 0\n        },\n        \"use_speaker_boost\": {\n          \"type\": \"boolean\",\n          \"description\": \"Enables speaker boost processing to increase voice clarity and reduce artifacts.\",\n       \
  \   \"default\": true\n        }\n      }\n    },\n    \"VoiceSample\": {\n      \"type\": \"object\",\n      \"description\": \"An audio sample associated with a voice, used for cloning and demonstration.\",\n      \"properties\": {\n        \"sample_id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the audio sample.\"\n        },\n        \"file_name\": {\n          \"type\": \"string\",\n          \"description\": \"Original file name of the uploaded sample.\"\n        },\n        \"mime_type\": {\n          \"type\": \"string\",\n          \"description\": \"MIME type of the audio sample.\",\n          \"pattern\": \"^audio/\"\n        },\n        \"size_bytes\": {\n          \"type\": \"integer\",\n          \"description\": \"Size of the audio sample file in bytes.\",\n          \"minimum\": 0\n        },\n        \"hash\": {\n          \"type\": \"string\",\n          \"description\": \"Hash of the audio sample content for integrity verification.\"\
  \n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/elevenlabs/refs/heads/main/json-schema/elevenlabs-voice-schema.json
tags: []
title: ElevenLabs Voice
---
