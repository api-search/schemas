---
description: ''
layout: schema
name: Poll
properties_list:
- description: Poll ID.
  name: id
  type: integer
- description: Poll title.
  name: title
  type: string
- description: Whether this is an anonymous poll.
  name: anonymous
  type: boolean
- description: Poll status.
  name: status
  type: string
- description: Type of poll. 1 - Poll, 2 - Advanced Poll, 3 - Quiz.
  name: poll_type
  type: integer
- description: List of questions in the poll.
  name: questions
  type: array
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-poll-schema.json
slug: zoom-meeting-poll
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Poll\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Poll ID.\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Poll title.\"\n    },\n    \"anonymous\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is an anonymous poll.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Poll status.\"\n    },\n    \"poll_type\": {\n      \"type\": \"integer\",\n      \"description\": \"Type of poll. 1 - Poll, 2 - Advanced Poll, 3 - Quiz.\"\n    },\n    \"questions\": {\n      \"type\": \"array\",\n      \"description\": \"List of questions in the poll.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-poll-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: Poll
---
