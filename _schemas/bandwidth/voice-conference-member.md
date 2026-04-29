---
description: ConferenceMember schema from Bandwidth voice API
layout: schema
name: ConferenceMember
properties_list:
- description: The call ID of the conference member
  name: callId
  type: string
- description: The conference ID
  name: conferenceId
  type: string
- description: The URL for this member resource
  name: memberUrl
  type: string
- description: Whether the member is muted
  name: mute
  type: boolean
- description: Whether the member is on hold
  name: hold
  type: boolean
- description: List of call IDs that this member is coaching
  name: callIdsToCoach
  type: array
provider_name: Bandwidth
provider_slug: bandwidth
schema_file: json-schema/voice-conference-member-schema.json
slug: voice-conference-member
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-conference-member-schema.json\",\n  \"title\": \"ConferenceMember\",\n  \"description\": \"ConferenceMember schema from Bandwidth voice API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"callId\": {\n      \"type\": \"string\",\n      \"description\": \"The call ID of the conference member\"\n    },\n    \"conferenceId\": {\n      \"type\": \"string\",\n      \"description\": \"The conference ID\"\n    },\n    \"memberUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL for this member resource\"\n    },\n    \"mute\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the member is muted\"\n    },\n    \"hold\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the member is on hold\"\n    },\n    \"callIdsToCoach\"\
  : {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"List of call IDs that this member is coaching\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/bandwidth/refs/heads/main/json-schema/voice-conference-member-schema.json
tags:
- Communications
- CPaaS
- Voice
- Messaging
- Telephony
- SMS
- MFA
title: ConferenceMember
---
