---
description: UpdateConferenceMemberRequest schema from Bandwidth voice API
layout: schema
name: UpdateConferenceMemberRequest
properties_list:
- description: Whether to mute the member
  name: mute
  type: boolean
- description: Whether to place the member on hold
  name: hold
  type: boolean
- description: List of call IDs that this member should coach
  name: callIdsToCoach
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-update-conference-member-request-schema.json
slug: voice-update-conference-member-request
source_filename: voice-update-conference-member-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-update-conference-member-request-schema.json\",\n  \"title\": \"UpdateConferenceMemberRequest\",\n  \"description\": \"UpdateConferenceMemberRequest schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"mute\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to mute the member\"\n    },\n    \"hold\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to place the member on hold\"\n    },\n    \"callIdsToCoach\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of call IDs that this member should coach\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-update-conference-member-request-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: UpdateConferenceMemberRequest
---
