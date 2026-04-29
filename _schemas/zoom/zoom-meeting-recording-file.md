---
description: ''
layout: schema
name: RecordingFile
properties_list:
- description: Recording file ID.
  name: id
  type: string
- description: Meeting ID.
  name: meeting_id
  type: string
- description: Recording start time.
  name: recording_start
  type: string
- description: Recording end time.
  name: recording_end
  type: string
- description: Recording file type.
  name: file_type
  type: string
- description: File extension.
  name: file_extension
  type: string
- description: File size in bytes.
  name: file_size
  type: number
- description: URL to download the recording file.
  name: download_url
  type: string
- description: URL to play the recording file.
  name: play_url
  type: string
- description: Recording status.
  name: status
  type: string
- description: Recording type.
  name: recording_type
  type: string
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-recording-file-schema.json
slug: zoom-meeting-recording-file
source_filename: zoom-meeting-recording-file-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecordingFile\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Recording file ID.\"\n    },\n    \"meeting_id\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting ID.\"\n    },\n    \"recording_start\": {\n      \"type\": \"string\",\n      \"description\": \"Recording start time.\"\n    },\n    \"recording_end\": {\n      \"type\": \"string\",\n      \"description\": \"Recording end time.\"\n    },\n    \"file_type\": {\n      \"type\": \"string\",\n      \"description\": \"Recording file type.\"\n    },\n    \"file_extension\": {\n      \"type\": \"string\",\n      \"description\": \"File extension.\"\n    },\n    \"file_size\": {\n      \"type\": \"number\",\n      \"description\": \"File size in bytes.\"\n    },\n    \"download_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to download\
  \ the recording file.\"\n    },\n    \"play_url\": {\n      \"type\": \"string\",\n      \"description\": \"URL to play the recording file.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Recording status.\"\n    },\n    \"recording_type\": {\n      \"type\": \"string\",\n      \"description\": \"Recording type.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-recording-file-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: RecordingFile
---
