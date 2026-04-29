---
description: RecordingDTO schema from Apache OpenMeetings REST API
layout: schema
name: RecordingDTO
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: hash
  type: string
- description: ''
  name: roomId
  type: integer
- description: ''
  name: status
  type: string
- description: ''
  name: interview
  type: boolean
- description: ''
  name: start
  type: string
- description: ''
  name: end
  type: string
- description: ''
  name: width
  type: integer
- description: ''
  name: height
  type: integer
- description: ''
  name: ownerId
  type: integer
- description: ''
  name: externalType
  type: string
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-recording-dto-schema.json
slug: apache-openmeetings-recording-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-recording-dto-schema.json\",\n  \"title\": \"RecordingDTO\",\n  \"description\": \"RecordingDTO schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"hash\": {\n      \"type\": \"string\"\n    },\n    \"roomId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"status\": {\n      \"type\": \"string\"\n    },\n    \"interview\": {\n      \"type\": \"boolean\"\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"width\": {\n      \"type\": \"integer\"\
  ,\n      \"format\": \"int32\"\n    },\n    \"height\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"ownerId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"externalType\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-recording-dto-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: RecordingDTO
---
