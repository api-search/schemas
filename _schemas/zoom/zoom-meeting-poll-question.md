---
description: ''
layout: schema
name: PollQuestion
properties_list:
- description: Question text.
  name: name
  type: string
- description: Question type.
  name: type
  type: string
- description: Whether an answer is required.
  name: answer_required
  type: boolean
- description: Available answer options.
  name: answers
  type: array
- description: Correct answers for quiz type polls.
  name: right_answers
  type: array
- description: Prompts for matching and rank order question types.
  name: prompts
  type: array
- description: Minimum rating value for rating scale questions.
  name: rating_min_value
  type: integer
- description: Maximum rating value for rating scale questions.
  name: rating_max_value
  type: integer
- description: Label for minimum rating value.
  name: rating_min_label
  type: string
- description: Label for maximum rating value.
  name: rating_max_label
  type: string
- description: Minimum characters for short/long answer questions.
  name: answer_min_character
  type: integer
- description: Maximum characters for short/long answer questions.
  name: answer_max_character
  type: integer
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-poll-question-schema.json
slug: zoom-meeting-poll-question
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PollQuestion\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Question text.\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Question type.\"\n    },\n    \"answer_required\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether an answer is required.\"\n    },\n    \"answers\": {\n      \"type\": \"array\",\n      \"description\": \"Available answer options.\"\n    },\n    \"right_answers\": {\n      \"type\": \"array\",\n      \"description\": \"Correct answers for quiz type polls.\"\n    },\n    \"prompts\": {\n      \"type\": \"array\",\n      \"description\": \"Prompts for matching and rank order question types.\"\n    },\n    \"rating_min_value\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum rating value for rating scale questions.\"\n    },\n    \"\
  rating_max_value\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum rating value for rating scale questions.\"\n    },\n    \"rating_min_label\": {\n      \"type\": \"string\",\n      \"description\": \"Label for minimum rating value.\"\n    },\n    \"rating_max_label\": {\n      \"type\": \"string\",\n      \"description\": \"Label for maximum rating value.\"\n    },\n    \"answer_min_character\": {\n      \"type\": \"integer\",\n      \"description\": \"Minimum characters for short/long answer questions.\"\n    },\n    \"answer_max_character\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum characters for short/long answer questions.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-poll-question-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: PollQuestion
---
