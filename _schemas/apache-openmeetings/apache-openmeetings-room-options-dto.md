---
description: RoomOptionsDTO schema from Apache OpenMeetings REST API
layout: schema
name: RoomOptionsDTO
properties_list:
- description: ''
  name: roomId
  type: integer
- description: ''
  name: externalRoomId
  type: string
- description: ''
  name: externalType
  type: string
- description: ''
  name: recordingId
  type: integer
- description: ''
  name: moderator
  type: boolean
- description: ''
  name: showAudioVideoTest
  type: boolean
- description: ''
  name: allowSameURLMultipleTimes
  type: boolean
- description: ''
  name: allowRecording
  type: boolean
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-room-options-dto-schema.json
slug: apache-openmeetings-room-options-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-room-options-dto-schema.json\",\n  \"title\": \"RoomOptionsDTO\",\n  \"description\": \"RoomOptionsDTO schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roomId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"externalRoomId\": {\n      \"type\": \"string\"\n    },\n    \"externalType\": {\n      \"type\": \"string\"\n    },\n    \"recordingId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"moderator\": {\n      \"type\": \"boolean\"\n    },\n    \"showAudioVideoTest\": {\n      \"type\": \"boolean\"\n    },\n    \"allowSameURLMultipleTimes\": {\n      \"type\": \"boolean\"\n    },\n    \"allowRecording\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-room-options-dto-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: RoomOptionsDTO
---
