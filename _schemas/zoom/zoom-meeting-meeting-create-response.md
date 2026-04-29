---
description: ''
layout: schema
name: MeetingCreateResponse
properties_list:
- description: Unique meeting instance ID.
  name: uuid
  type: string
- description: Meeting ID (meeting number).
  name: id
  type: integer
- description: ID of the meeting host.
  name: host_id
  type: string
- description: Email address of the meeting host.
  name: host_email
  type: string
- description: Meeting topic.
  name: topic
  type: string
- description: Meeting status.
  name: status
  type: string
- description: Meeting start time.
  name: start_time
  type: string
- description: Meeting duration in minutes.
  name: duration
  type: integer
- description: Timezone of the meeting.
  name: timezone
  type: string
- description: Meeting agenda.
  name: agenda
  type: string
- description: Time the meeting was created.
  name: created_at
  type: string
- description: URL for the host to start the meeting.
  name: start_url
  type: string
- description: URL for participants to join the meeting.
  name: join_url
  type: string
- description: Meeting passcode.
  name: password
  type: string
- description: H.323/SIP room system passcode.
  name: h323_password
  type: string
- description: Password for PSTN dial-in.
  name: pstn_password
  type: string
- description: Encrypted passcode for the meeting URL.
  name: encrypted_password
  type: string
- description: ''
  name: occurrences
  type: array
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-meeting-create-response-schema.json
slug: zoom-meeting-meeting-create-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeetingCreateResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique meeting instance ID.\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting ID (meeting number).\"\n    },\n    \"host_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the meeting host.\"\n    },\n    \"host_email\": {\n      \"type\": \"string\",\n      \"description\": \"Email address of the meeting host.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting topic.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting status.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting start time.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\":\
  \ \"Meeting duration in minutes.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone of the meeting.\"\n    },\n    \"agenda\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting agenda.\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"description\": \"Time the meeting was created.\"\n    },\n    \"start_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL for the host to start the meeting.\"\n    },\n    \"join_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL for participants to join the meeting.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting passcode.\"\n    },\n    \"h323_password\": {\n      \"type\": \"string\",\n      \"description\": \"H.323/SIP room system passcode.\"\n    },\n    \"pstn_password\": {\n      \"type\": \"string\",\n      \"description\": \"Password for PSTN dial-in.\"\n    },\n    \"encrypted_password\":\
  \ {\n      \"type\": \"string\",\n      \"description\": \"Encrypted passcode for the meeting URL.\"\n    },\n    \"occurrences\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-meeting-create-response-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: MeetingCreateResponse
---
