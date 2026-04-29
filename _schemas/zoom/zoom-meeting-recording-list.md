---
description: ''
layout: schema
name: RecordingList
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
- description: Meeting start time.
  name: start_time
  type: string
- description: Timezone.
  name: timezone
  type: string
- description: Meeting duration in minutes.
  name: duration
  type: integer
- description: Total file size of all recordings in bytes.
  name: total_size
  type: integer
- description: Number of recording files.
  name: recording_count
  type: integer
- description: Share URL for the recording.
  name: share_url
  type: string
- description: ''
  name: recording_files
  type: array
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-recording-list-schema.json
slug: zoom-meeting-recording-list
source_filename: zoom-meeting-recording-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecordingList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"uuid\": {\n      \"type\": \"string\",\n      \"description\": \"Unique meeting instance ID.\"\n    },\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting ID.\"\n    },\n    \"host_id\": {\n      \"type\": \"string\",\n      \"description\": \"Host user ID.\"\n    },\n    \"host_email\": {\n      \"type\": \"string\",\n      \"description\": \"Host email address.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting topic.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting start time.\"\n    },\n    \"timezone\": {\n      \"type\": \"string\",\n      \"description\": \"Timezone.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting duration in minutes.\"\n    },\n    \"total_size\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Total file size of all recordings in bytes.\"\n    },\n    \"recording_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of recording files.\"\n    },\n    \"share_url\": {\n      \"type\": \"string\",\n      \"description\": \"Share URL for the recording.\"\n    },\n    \"recording_files\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-recording-list-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: RecordingList
---
