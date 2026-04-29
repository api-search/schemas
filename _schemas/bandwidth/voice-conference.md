---
description: Conference schema from Bandwidth voice API
layout: schema
name: Conference
properties_list:
- description: The unique identifier for the conference
  name: id
  type: string
- description: The user-defined name of the conference
  name: name
  type: string
- description: The time the conference was created
  name: createdTime
  type: string
- description: The time the conference ended
  name: completedTime
  type: string
- description: Custom tag attached to the conference
  name: tag
  type: string
- description: List of currently active conference members
  name: activeMembers
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-conference-schema.json
slug: voice-conference
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-conference-schema.json\",\n  \"title\": \"Conference\",\n  \"description\": \"Conference schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier for the conference\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The user-defined name of the conference\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the conference was created\"\n    },\n    \"completedTime\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"The time the conference ended\"\n    },\n    \"tag\": {\n      \"type\": \"string\",\n      \"description\": \"Custom tag attached\
  \ to the conference\"\n    },\n    \"activeMembers\": {\n      \"type\": \"array\",\n      \"description\": \"List of currently active conference members\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/ConferenceMember\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-conference-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: Conference
---
