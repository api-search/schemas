---
description: ''
layout: schema
name: Participant
properties_list:
- description: Participant UUID.
  name: id
  type: string
- description: Participant user ID if the participant is a Zoom user.
  name: user_id
  type: string
- description: Participant display name.
  name: name
  type: string
- description: Participant email address.
  name: user_email
  type: string
- description: Time the participant joined the meeting.
  name: join_time
  type: string
- description: Time the participant left the meeting.
  name: leave_time
  type: string
- description: Participant duration in the meeting (seconds).
  name: duration
  type: integer
- description: Registrant ID if the participant registered.
  name: registrant_id
  type: string
- description: Whether failover occurred for this participant.
  name: failover
  type: boolean
- description: Participant status.
  name: status
  type: string
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-participant-schema.json
slug: zoom-meeting-participant
source_filename: zoom-meeting-participant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Participant\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Participant UUID.\"\n    },\n    \"user_id\": {\n      \"type\": \"string\",\n      \"description\": \"Participant user ID if the participant is a Zoom user.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Participant display name.\"\n    },\n    \"user_email\": {\n      \"type\": \"string\",\n      \"description\": \"Participant email address.\"\n    },\n    \"join_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time the participant joined the meeting.\"\n    },\n    \"leave_time\": {\n      \"type\": \"string\",\n      \"description\": \"Time the participant left the meeting.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Participant duration in the meeting (seconds).\"\n\
  \    },\n    \"registrant_id\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant ID if the participant registered.\"\n    },\n    \"failover\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether failover occurred for this participant.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Participant status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-participant-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: Participant
---
