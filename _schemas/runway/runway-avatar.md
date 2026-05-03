---
description: Represents an avatar persona in the Runway Characters system. Avatars are persistent conversational video agents with defined appearance, voice, and personality, created from a single reference image.
layout: schema
name: Runway Avatar
properties_list:
- description: The unique identifier for the avatar.
  name: id
  type: string
- description: A human-readable name for the avatar persona.
  name: name
  type: string
- description: The HTTPS URL of the reference image used for the avatar's appearance. Any visual style works, from photorealistic humans to animated mascots.
  name: referenceImage
  type: string
- description: Instructions defining the avatar's personality, behavior, and conversational style.
  name: personality
  type: string
- description: Voice configuration for the avatar.
  name: voice
  type: object
- description: An optional opening message that the avatar speaks when a session starts.
  name: openingMessage
  type: string
- description: List of knowledge document IDs attached to the avatar, providing additional context during conversations.
  name: documentIds
  type: array
- description: The ISO 8601 timestamp when the avatar was created.
  name: createdAt
  type: string
provider_name: Runway
provider_slug: runway
schema_file: json-schema/runway-avatar-schema.json
slug: runway-avatar
source_filename: runway-avatar-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://api.dev.runwayml.com/schemas/runway/avatar.json\",\n  \"title\": \"Runway Avatar\",\n  \"description\": \"Represents an avatar persona in the Runway Characters system. Avatars are persistent conversational video agents with defined appearance, voice, and personality, created from a single reference image.\",\n  \"type\": \"object\",\n  \"required\": [\"id\", \"name\"],\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"description\": \"The unique identifier for the avatar.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable name for the avatar persona.\",\n      \"minLength\": 1\n    },\n    \"referenceImage\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The HTTPS URL of the reference image used for the avatar's appearance. Any visual style works,\
  \ from photorealistic humans to animated mascots.\"\n    },\n    \"personality\": {\n      \"type\": \"string\",\n      \"description\": \"Instructions defining the avatar's personality, behavior, and conversational style.\"\n    },\n    \"voice\": {\n      \"$ref\": \"#/$defs/VoiceConfig\",\n      \"description\": \"Voice configuration for the avatar.\"\n    },\n    \"openingMessage\": {\n      \"type\": \"string\",\n      \"description\": \"An optional opening message that the avatar speaks when a session starts.\"\n    },\n    \"documentIds\": {\n      \"type\": \"array\",\n      \"description\": \"List of knowledge document IDs attached to the avatar, providing additional context during conversations.\",\n      \"maxItems\": 50,\n      \"items\": {\n        \"type\": \"string\",\n        \"format\": \"uuid\"\n      }\n    },\n    \"createdAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The ISO 8601 timestamp when the avatar was created.\"\
  \n    }\n  },\n  \"$defs\": {\n    \"VoiceConfig\": {\n      \"type\": \"object\",\n      \"description\": \"Configuration for the avatar's voice, specifying the voice provider and preset.\",\n      \"required\": [\"type\", \"presetId\"],\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"description\": \"The voice provider type.\",\n          \"enum\": [\"runway-live-preset\"]\n        },\n        \"presetId\": {\n          \"type\": \"string\",\n          \"description\": \"The identifier of the voice preset to use for the avatar.\"\n        }\n      }\n    },\n    \"RealtimeSession\": {\n      \"type\": \"object\",\n      \"description\": \"A live WebRTC session connecting a user to an avatar for real-time conversational interaction. Sessions have a maximum duration of 5 minutes.\",\n      \"required\": [\"id\", \"status\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n       \
  \   \"description\": \"The unique identifier of the session.\"\n        },\n        \"status\": {\n          \"type\": \"string\",\n          \"description\": \"The current status of the session.\",\n          \"enum\": [\"PENDING\", \"READY\", \"ACTIVE\", \"ENDED\"]\n        },\n        \"model\": {\n          \"type\": \"string\",\n          \"description\": \"The model type used for the session.\",\n          \"enum\": [\"gwm1_avatars\"]\n        },\n        \"serverUrl\": {\n          \"type\": \"string\",\n          \"format\": \"uri\",\n          \"description\": \"The WebRTC server URL to connect to.\"\n        },\n        \"token\": {\n          \"type\": \"string\",\n          \"description\": \"The one-time authentication token for the WebRTC connection.\"\n        },\n        \"roomName\": {\n          \"type\": \"string\",\n          \"description\": \"The name of the WebRTC room to join.\"\n        },\n        \"maxSessionDurationSeconds\": {\n          \"type\": \"integer\"\
  ,\n          \"description\": \"Maximum session duration in seconds.\",\n          \"maximum\": 300\n        }\n      }\n    },\n    \"Document\": {\n      \"type\": \"object\",\n      \"description\": \"A domain-specific knowledge document that avatars can reference during conversations to provide accurate, contextual responses.\",\n      \"required\": [\"id\", \"name\"],\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"format\": \"uuid\",\n          \"description\": \"The unique identifier of the document.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"A human-readable name for the knowledge document.\"\n        },\n        \"content\": {\n          \"type\": \"string\",\n          \"description\": \"The text content of the knowledge document. Each avatar supports up to 50,000 tokens of knowledge across all attached documents.\"\n        },\n        \"createdAt\": {\n          \"type\": \"string\"\
  ,\n          \"format\": \"date-time\",\n          \"description\": \"The ISO 8601 timestamp when the document was uploaded.\"\n        }\n      }\n    },\n    \"PresetAvatar\": {\n      \"type\": \"string\",\n      \"description\": \"Available preset avatar identifiers for quick session creation without custom avatar setup.\",\n      \"enum\": [\n        \"game-character\",\n        \"music-superstar\",\n        \"game-character-man\",\n        \"cat-character\",\n        \"influencer\",\n        \"tennis-coach\",\n        \"human-resource\",\n        \"fashion-designer\",\n        \"cooking-teacher\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/runway/refs/heads/main/json-schema/runway-avatar-schema.json
tags:
- Video Generation
- Image Generation
- Artificial Intelligence
- Machine Learning
- Generative AI
- Avatars
- Characters
- WebRTC
- Creative Tools
title: Runway Avatar
---
