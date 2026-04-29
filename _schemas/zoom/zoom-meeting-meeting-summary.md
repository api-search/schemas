---
description: ''
layout: schema
name: MeetingSummary
properties_list:
- description: Unique meeting instance ID.
  name: uuid
  type: string
- description: Meeting ID (meeting number).
  name: id
  type: integer
- description: ID of the user who is the meeting host.
  name: host_id
  type: string
- description: Meeting topic.
  name: topic
  type: string
- description: Meeting start time in UTC.
  name: start_time
  type: string
- description: Meeting duration in minutes.
  name: duration
  type: integer
- description: Timezone for the meeting start time.
  name: timezone
  type: string
- description: Time the meeting was created.
  name: created_at
  type: string
- description: URL for participants to join the meeting.
  name: join_url
  type: string
- description: Meeting agenda or description.
  name: agenda
  type: string
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-meeting-summary-schema.json
slug: zoom-meeting-meeting-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeetingSummary\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique meeting instance ID.\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting ID (meeting number).\"\n    },\n    \"host_id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the user who is the meeting host.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting topic.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting start time in UTC.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting duration in minutes.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for the meeting start time.\"\n    },\n    \"created_at\": {\n      \"type\": \"\
  string\",\n      \"description\": \"Time the meeting was created.\"\n    },\n    \"join_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL for participants to join the meeting.\"\n    },\n    \"agenda\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting agenda or description.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-meeting-summary-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: MeetingSummary
---
