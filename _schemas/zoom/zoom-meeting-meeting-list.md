---
description: ''
layout: schema
name: MeetingList
properties_list:
- description: Total number of pages.
  name: page_count
  type: integer
- description: Current page number.
  name: page_number
  type: integer
- description: Number of records per page.
  name: page_size
  type: integer
- description: Total number of meeting records.
  name: total_records
  type: integer
- description: Token for the next page of results.
  name: next_page_token
  type: string
- description: List of meeting objects.
  name: meetings
  type: array
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-meeting-list-schema.json
slug: zoom-meeting-meeting-list
source_filename: zoom-meeting-meeting-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MeetingList\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"page_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of pages.\"\n    },\n    \"page_number\": {\n      \"type\": \"integer\",\n      \"description\": \"Current page number.\"\n    },\n    \"page_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of records per page.\"\n    },\n    \"total_records\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of meeting records.\"\n    },\n    \"next_page_token\": {\n      \"type\": \"string\",\n      \"description\": \"Token for the next page of results.\"\n    },\n    \"meetings\": {\n      \"type\": \"array\",\n      \"description\": \"List of meeting objects.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-meeting-list-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: MeetingList
---
