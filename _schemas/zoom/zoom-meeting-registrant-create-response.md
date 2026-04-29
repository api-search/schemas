---
description: ''
layout: schema
name: RegistrantCreateResponse
properties_list:
- description: Meeting ID.
  name: id
  type: integer
- description: Registrant ID.
  name: registrant_id
  type: string
- description: Meeting start time.
  name: start_time
  type: string
- description: Meeting topic.
  name: topic
  type: string
- description: Unique join URL for this registrant.
  name: join_url
  type: string
- description: Participant PIN code for phone dial-in.
  name: participant_pin_code
  type: integer
provider_name: Zoom
provider_slug: zoom
schema_file: json-schema/zoom-meeting-registrant-create-response-schema.json
slug: zoom-meeting-registrant-create-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RegistrantCreateResponse\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"description\": \"Meeting ID.\"\n    },\n    \"registrant_id\": {\n      \"type\": \"string\",\n      \"description\": \"Registrant ID.\"\n    },\n    \"start_time\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting start time.\"\n    },\n    \"topic\": {\n      \"type\": \"string\",\n      \"description\": \"Meeting topic.\"\n    },\n    \"join_url\": {\n      \"type\": \"string\",\n      \"description\": \"Unique join URL for this registrant.\"\n    },\n    \"participant_pin_code\": {\n      \"type\": \"integer\",\n      \"description\": \"Participant PIN code for phone dial-in.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoom/refs/heads/main/json-schema/zoom-meeting-registrant-create-response-schema.json
tags:
- Chat
- Collaboration
- Communications
- Meetings
- Video Conferencing
- Videos
- Webinars
title: RegistrantCreateResponse
---
