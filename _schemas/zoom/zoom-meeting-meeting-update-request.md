---
description: ''
layout: schema
name: MeetingUpdateRequest
properties_list:
- description: Meeting topic.
  name: topic
  type: string
- description: Meeting start time.
  name: start_time
  type: string
- description: Meeting duration in minutes.
  name: duration
  type: integer
- description: Email address or user ID to schedule meeting on behalf of.
  name: schedule_for
  type: string
- description: Timezone for start_time.
  name: timezone
  type: string
- description: Meeting passcode.
  name: password
  type: string
- description: Meeting description.
  name: agenda
  type: string
- description: ''
  name: tracking_fields
  type: array
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-meeting-update-request-schema.json
slug: zoom-meeting-meeting-update-request
source_filename: zoom-meeting-meeting-update-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeetingUpdateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting topic.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting start time.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting duration in minutes.\"\n    },\n    \"schedule_for\": {\n      \"type\": \"string\",\n      \"description\": \"Email address or user ID to schedule meeting on behalf of.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone for start_time.\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting passcode.\"\n    },\n    \"agenda\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting description.\"\n    },\n    \"tracking_fields\": {\n      \"type\"\
  : \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-meeting-update-request-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: MeetingUpdateRequest
---
