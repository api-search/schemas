---
description: ''
layout: schema
name: PollCreateRequest
properties_list:
- description: Poll title. Maximum 64 characters.
  name: title
  type: string
- description: Whether this is an anonymous poll.
  name: anonymous
  type: boolean
- description: Type of poll. 1 - Poll, 2 - Advanced Poll, 3 - Quiz.
  name: poll_type
  type: integer
- description: List of questions for the poll.
  name: questions
  type: array
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-poll-create-request-schema.json
slug: zoom-meeting-poll-create-request
source_filename: zoom-meeting-poll-create-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PollCreateRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Poll title. Maximum 64 characters.\"\n    },\n    \"anonymous\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an anonymous poll.\"\n    },\n    \"poll_type\": {\n      \"type\": \"integer\",\n      \"description\": \"Type of poll. 1 - Poll, 2 - Advanced Poll, 3 - Quiz.\"\n    },\n    \"questions\": {\n      \"type\": \"array\",\n      \"description\": \"List of questions for the poll.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-poll-create-request-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: PollCreateRequest
---
