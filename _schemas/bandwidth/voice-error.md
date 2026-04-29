---
description: Error schema from Bandwidth voice API
layout: schema
name: Error
properties_list:
- description: The error type URI
  name: type
  type: string
- description: A human-readable description of the error
  name: description
  type: string
- description: The unique error identifier
  name: id
  type: string
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-error-schema.json
slug: voice-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-error-schema.json\",\n  \"title\": \"Error\",\n  \"description\": \"Error schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The error type URI\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable description of the error\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique error identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-error-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Error
---
