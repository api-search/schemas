---
description: ''
layout: schema
name: ErrorResponse
properties_list:
- description: Error code.
  name: code
  type: integer
- description: Error message.
  name: message
  type: string
- description: Detailed error messages.
  name: errors
  type: array
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-error-response-schema.json
slug: zoom-meeting-error-response
source_filename: zoom-meeting-error-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"code\": {\n      \"type\": \"integer\",\n      \"description\": \"Error code.\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed error messages.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-error-response-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: ErrorResponse
---
