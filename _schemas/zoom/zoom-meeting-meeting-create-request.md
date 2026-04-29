---
description: ''
layout: schema
name: MeetingCreateRequest
properties_list:
- description: Meeting topic. Maximum 200 characters.
  name: topic
  type: string
- description: Whether to create a pre-scheduled meeting.
  name: pre_schedule
  type: boolean
- description: Meeting start time. Only used for scheduled meetings (type 2) and recurring meetings with a fixed time (type 8). Use UTC format such as 2023-11-25T12:00:00Z.
  name: start_time
  type: string
- description: Meeting duration in minutes. Used for scheduled meetings only.
  name: duration
  type: integer
- description: Email address or user ID to schedule the meeting on behalf of.
  name: schedule_for
  type: string
- description: Timezone to format start_time (e.g., America/Los_Angeles). If not provided, defaults to the meeting host's timezone.
  name: timezone
  type: string
- description: 'Meeting passcode. May only contain the following characters: a-z A-Z 0-9 @ - _ *. Maximum 10 characters.'
  name: password
  type: string
- description: Use the default passcode set in account settings.
  name: default_password
  type: boolean
- description: Meeting description. Maximum 2000 characters.
  name: agenda
  type: string
- description: Tracking fields for the meeting.
  name: tracking_fields
  type: array
- description: Meeting template ID to use.
  name: template_id
  type: string
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-meeting-create-request-schema.json
slug: zoom-meeting-meeting-create-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeetingCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting topic. Maximum 200 characters.\"\n    },\n    \"pre_schedule\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to create a pre-scheduled meeting.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting start time. Only used for scheduled meetings (type 2) and recurring meetings with a fixed time (type 8). Use UTC format such as 2023-11-25T12:00:00Z.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting duration in minutes. Used for scheduled meetings only.\"\n    },\n    \"schedule_for\": {\n      \"type\": \"string\",\n      \"description\": \"Email address or user ID to schedule the meeting on behalf of.\"\n    },\n    \"timezone\": {\n      \"\
  type\": \"string\",\n      \"description\": \"Timezone to format start_time (e.g., America/Los_Angeles). If not provided, defaults to the meeting host's timezone.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting passcode. May only contain the following characters: a-z A-Z 0-9 @ - _ *. Maximum 10 characters.\"\n    },\n    \"default_password\": {\n      \"type\": \"boolean\",\n      \"description\": \"Use the default passcode set in account settings.\"\n    },\n    \"agenda\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting description. Maximum 2000 characters.\"\n    },\n    \"tracking_fields\": {\n      \"type\": \"array\",\n      \"description\": \"Tracking fields for the meeting.\"\n    },\n    \"template_id\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting template ID to use.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-meeting-create-request-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: MeetingCreateRequest
---
