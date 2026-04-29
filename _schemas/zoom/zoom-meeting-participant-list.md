---
description: ''
layout: schema
name: ParticipantList
properties_list:
- description: ''
  name: page_count
  type: integer
- description: ''
  name: page_size
  type: integer
- description: ''
  name: total_records
  type: integer
- description: ''
  name: next_page_token
  type: string
- description: ''
  name: participants
  type: array
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-participant-list-schema.json
slug: zoom-meeting-participant-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ParticipantList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"page_count\": {\n      \"type\": \"integer\"\n    },\n    \"page_size\": {\n      \"type\": \"integer\"\n    },\n    \"total_records\": {\n      \"type\": \"integer\"\n    },\n    \"next_page_token\": {\n      \"type\": \"string\"\n    },\n    \"participants\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-participant-list-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: ParticipantList
---
