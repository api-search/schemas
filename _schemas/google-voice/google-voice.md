---
description: JSON Schema for Google Voice related objects managed through Google Workspace Admin SDK.
layout: schema
name: Google Voice API Schema
properties_list: []
provider_name: Google Voice
provider_slug: google-voice
schema_file: json-schema/google-voice.json
slug: google-voice
source_filename: google-voice.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-voice/refs/heads/main/json-schema/google-voice.json\",\n  \"title\": \"Google Voice API Schema\",\n  \"description\": \"JSON Schema for Google Voice related objects managed through Google Workspace Admin SDK.\",\n  \"type\": \"object\",\n  \"$defs\": {\n    \"User\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the user.\"\n        },\n        \"primaryEmail\": {\n          \"type\": \"string\",\n          \"format\": \"email\",\n          \"description\": \"The user's primary email address.\"\n        },\n        \"name\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"givenName\": {\n              \"type\": \"string\"\n            },\n            \"familyName\": {\n              \"type\": \"\
  string\"\n            },\n            \"fullName\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"phones\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"value\": {\n                \"type\": \"string\",\n                \"description\": \"Phone number.\"\n              },\n              \"type\": {\n                \"type\": \"string\",\n                \"description\": \"Type of phone.\"\n              },\n              \"primary\": {\n                \"type\": \"boolean\"\n              }\n            }\n          }\n        },\n        \"isAdmin\": {\n          \"type\": \"boolean\"\n        }\n      }\n    },\n    \"Building\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"buildingId\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier for the building.\"\n        },\n        \"buildingName\"\
  : {\n          \"type\": \"string\",\n          \"description\": \"Name of the building.\"\n        },\n        \"description\": {\n          \"type\": \"string\",\n          \"description\": \"Description of the building.\"\n        },\n        \"address\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"addressLines\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"locality\": {\n              \"type\": \"string\"\n            },\n            \"administrativeArea\": {\n              \"type\": \"string\"\n            },\n            \"postalCode\": {\n              \"type\": \"string\"\n            },\n            \"regionCode\": {\n              \"type\": \"string\"\n            }\n          }\n        },\n        \"floorNames\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"string\"\n          }\n        }\n    \
  \  }\n    },\n    \"VoiceSettings\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"voicemailGreeting\": {\n          \"type\": \"string\",\n          \"description\": \"Custom voicemail greeting.\"\n        },\n        \"doNotDisturb\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether do-not-disturb is enabled.\"\n        },\n        \"callForwarding\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"enabled\": {\n              \"type\": \"boolean\"\n            },\n            \"forwardTo\": {\n              \"type\": \"string\",\n              \"description\": \"Phone number to forward calls to.\"\n            }\n          }\n        },\n        \"voicemailTranscription\": {\n          \"type\": \"boolean\",\n          \"description\": \"Whether voicemail transcription is enabled.\"\n        }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-voice/refs/heads/main/json-schema/google-voice.json
tags:
- Google Voice
- Messaging
- Phone
- Telecommunications
- Voice
- Voicemail
- VoIP
title: Google Voice API Schema
---
