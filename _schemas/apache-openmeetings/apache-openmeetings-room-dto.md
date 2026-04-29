---
description: RoomDTO schema from Apache OpenMeetings REST API
layout: schema
name: RoomDTO
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: tag
  type: string
- description: ''
  name: comment
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: capacity
  type: integer
- description: ''
  name: appointment
  type: boolean
- description: ''
  name: confno
  type: string
- description: ''
  name: demo
  type: boolean
- description: ''
  name: closed
  type: boolean
- description: ''
  name: demoTime
  type: integer
- description: ''
  name: externalId
  type: string
- description: ''
  name: externalType
  type: string
- description: ''
  name: redirectUrl
  type: string
- description: ''
  name: moderated
  type: boolean
- description: ''
  name: waitModerator
  type: boolean
- description: ''
  name: allowUserQuestions
  type: boolean
- description: ''
  name: allowRecording
  type: boolean
- description: ''
  name: waitRecording
  type: boolean
- description: ''
  name: audioOnly
  type: boolean
- description: ''
  name: hiddenElements
  type: array
- description: ''
  name: files
  type: array
- description: ''
  name: public
  type: boolean
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-room-dto-schema.json
slug: apache-openmeetings-room-dto
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-room-dto-schema.json\",\n  \"title\": \"RoomDTO\",\n  \"description\": \"RoomDTO schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"tag\": {\n      \"type\": \"string\"\n    },\n    \"comment\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"CONFERENCE\",\n        \"PRESENTATION\",\n        \"INTERVIEW\"\n      ]\n    },\n    \"capacity\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"appointment\": {\n      \"type\": \"boolean\"\n    },\n    \"confno\": {\n      \"type\": \"string\"\n    },\n    \"demo\"\
  : {\n      \"type\": \"boolean\"\n    },\n    \"closed\": {\n      \"type\": \"boolean\"\n    },\n    \"demoTime\": {\n      \"type\": \"integer\",\n      \"format\": \"int32\"\n    },\n    \"externalId\": {\n      \"type\": \"string\"\n    },\n    \"externalType\": {\n      \"type\": \"string\"\n    },\n    \"redirectUrl\": {\n      \"type\": \"string\"\n    },\n    \"moderated\": {\n      \"type\": \"boolean\"\n    },\n    \"waitModerator\": {\n      \"type\": \"boolean\"\n    },\n    \"allowUserQuestions\": {\n      \"type\": \"boolean\"\n    },\n    \"allowRecording\": {\n      \"type\": \"boolean\"\n    },\n    \"waitRecording\": {\n      \"type\": \"boolean\"\n    },\n    \"audioOnly\": {\n      \"type\": \"boolean\"\n    },\n    \"hiddenElements\": {\n      \"uniqueItems\": true,\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\n          \"TOP_BAR\",\n          \"CHAT\",\n          \"ACTIVITIES\",\n          \"FILES\",\n      \
  \    \"ACTION_MENU\",\n          \"POLL_MENU\",\n          \"SCREEN_SHARING\",\n          \"WHITEBOARD\",\n          \"MICROPHONE_STATUS\",\n          \"USER_COUNT\"\n        ]\n      }\n    },\n    \"files\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RoomFileDTO\"\n      }\n    },\n    \"public\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-room-dto-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: RoomDTO
---
