---
description: JSON Schema for the Google Assistant API device model, device instance, and conversation objects.
layout: schema
name: Google Assistant API Schema
properties_list: []
provider_name: Google Assistant
provider_slug: google-assistant
schema_file: json-schema/google-assistant.json
slug: google-assistant
source_filename: google-assistant.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-assistant/refs/heads/main/json-schema/google-assistant.json\",\n  \"title\": \"Google Assistant API Schema\",\n  \"description\": \"JSON Schema for the Google Assistant API device model, device instance, and conversation objects.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"DeviceModel\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"deviceModelId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the device model.\"\n        },\n        \"projectId\": {\n          \"type\": \"string\",\n          \"description\": \"The Google Cloud project ID.\"\n        },\n        \"name\": {\n          \"type\": \"string\",\n          \"description\": \"Display name of the device model.\"\n        },\n        \"deviceType\": {\n          \"type\": \"string\",\n          \"enum\": [\"LIGHT\"\
  , \"SWITCH\", \"OUTLET\", \"SPEAKER\", \"TV\", \"AUTO\"],\n          \"description\": \"The type of device.\"\n        },\n        \"traits\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          },\n          \"description\": \"List of supported device traits.\"\n        },\n        \"manifest\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"manufacturer\": {\n              \"type\": \"string\"\n            },\n            \"productName\": {\n              \"type\": \"string\"\n            },\n            \"deviceDescription\": {\n              \"type\": \"string\"\n            }\n          }\n        }\n      }\n    },\n    \"DeviceInstance\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the device instance.\"\n        },\n        \"deviceModelId\": {\n          \"type\": \"string\",\n   \
  \       \"description\": \"The device model this instance belongs to.\"\n        },\n        \"nickname\": {\n          \"type\": \"string\",\n          \"description\": \"Nickname for the device.\"\n        },\n        \"clientType\": {\n          \"type\": \"string\",\n          \"description\": \"Client type of the device.\"\n        }\n      }\n    },\n    \"AssistRequest\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"config\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"textInput\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"text\": {\n                  \"type\": \"string\",\n                  \"description\": \"Text query to the Assistant.\"\n                }\n              }\n            },\n            \"audioInConfig\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"encoding\": {\n                  \"type\": \"string\",\n      \
  \            \"enum\": [\"LINEAR16\", \"FLAC\"]\n                },\n                \"sampleRateHertz\": {\n                  \"type\": \"integer\"\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"AssistResponse\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"dialogStateOut\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"supplementalDisplayText\": {\n              \"type\": \"string\",\n              \"description\": \"Text response from the Assistant.\"\n            },\n            \"conversationState\": {\n              \"type\": \"string\",\n              \"description\": \"Opaque conversation state.\"\n            },\n            \"microphoneMode\": {\n              \"type\": \"string\",\n              \"enum\": [\"CLOSE_MICROPHONE\", \"DIALOG_FOLLOW_ON\"]\n            }\n          }\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-assistant/refs/heads/main/json-schema/google-assistant.json
tags:
- Actions on Google
- Conversational AI
- Google Assistant
- Natural Language
- Smart Home
- Voice Assistant
title: Google Assistant API Schema
---
