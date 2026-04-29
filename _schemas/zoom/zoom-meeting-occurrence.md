---
description: Meeting occurrence information for recurring meetings.
layout: schema
name: Occurrence
properties_list:
- description: Occurrence ID.
  name: occurrence_id
  type: string
- description: Start time of this occurrence.
  name: start_time
  type: string
- description: Duration of this occurrence in minutes.
  name: duration
  type: integer
- description: Occurrence status.
  name: status
  type: string
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-occurrence-schema.json
slug: zoom-meeting-occurrence
source_filename: zoom-meeting-occurrence-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Occurrence\",\n  \"type\": \"object\",\n  \"description\": \"Meeting occurrence information for recurring meetings.\",\n  \"properties\": {\n    \"occurrence_id\": {\n      \"type\": \"string\",\n      \"description\": \"Occurrence ID.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Start time of this occurrence.\"\n    },\n    \"duration\": {\n      \"type\": \"integer\",\n      \"description\": \"Duration of this occurrence in minutes.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Occurrence status.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-occurrence-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: Occurrence
---
