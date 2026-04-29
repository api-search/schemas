---
description: ''
layout: schema
name: PastMeetingDetails
properties_list:
- description: Unique meeting instance ID.
  name: uuid
  type: string
- description: Meeting ID.
  name: id
  type: integer
- description: Host user ID.
  name: host_id
  type: string
- description: Host email address.
  name: host_email
  type: string
- description: Meeting topic.
  name: topic
  type: string
- description: Display name of the meeting host.
  name: user_name
  type: string
- description: Meeting start time.
  name: start_time
  type: string
- description: Meeting end time.
  name: end_time
  type: string
- description: Meeting duration in minutes.
  name: duration
  type: integer
- description: Total meeting minutes across all participants.
  name: total_minutes
  type: integer
- description: Number of participants.
  name: participants_count
  type: integer
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-past-meeting-details-schema.json
slug: zoom-meeting-past-meeting-details
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PastMeetingDetails\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique meeting instance ID.\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting ID.\"\n    },\n    \"host_id\": {\n      \"type\": \"string\",\n      \"description\": \"Host user ID.\"\n    },\n    \"host_email\": {\n      \"type\": \"string\",\n      \"description\": \"Host email address.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting topic.\"\n    },\n    \"user_name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the meeting host.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting start time.\"\n    },\n    \"end_time\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting end time.\"\n \
  \   },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting duration in minutes.\"\n    },\n    \"total_minutes\": {\n      \"type\": \"integer\",\n      \"description\": \"Total meeting minutes across all participants.\"\n    },\n    \"participants_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of participants.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-past-meeting-details-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: PastMeetingDetails
---
