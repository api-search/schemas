---
description: AppointmentDTO schema from Apache OpenMeetings REST API
layout: schema
name: AppointmentDTO
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: title
  type: string
- description: ''
  name: location
  type: string
- description: ''
  name: start
  type: string
- description: ''
  name: end
  type: string
- description: ''
  name: description
  type: string
- description: ''
  name: owner
  type: object
- description: ''
  name: inserted
  type: string
- description: ''
  name: updated
  type: string
- description: ''
  name: deleted
  type: boolean
- description: ''
  name: reminder
  type: string
- description: ''
  name: room
  type: object
- description: ''
  name: icalId
  type: string
- description: ''
  name: meetingMembers
  type: array
- description: ''
  name: languageId
  type: integer
- description: ''
  name: password
  type: string
- description: ''
  name: passwordProtected
  type: boolean
- description: ''
  name: connectedEvent
  type: boolean
- description: ''
  name: reminderEmailSend
  type: boolean
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-appointment-dto-schema.json
slug: apache-openmeetings-appointment-dto
source_filename: apache-openmeetings-appointment-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-appointment-dto-schema.json\",\n  \"title\": \"AppointmentDTO\",\n  \"description\": \"AppointmentDTO schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"title\": {\n      \"type\": \"string\"\n    },\n    \"location\": {\n      \"type\": \"string\"\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"description\": {\n      \"type\": \"string\"\n    },\n    \"owner\": {\n      \"$ref\": \"#/components/schemas/UserDTO\"\n    },\n    \"inserted\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n \
  \   \"updated\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"deleted\": {\n      \"type\": \"boolean\"\n    },\n    \"reminder\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"NONE\",\n        \"EMAIL\",\n        \"ICAL\"\n      ]\n    },\n    \"room\": {\n      \"$ref\": \"#/components/schemas/RoomDTO\"\n    },\n    \"icalId\": {\n      \"type\": \"string\"\n    },\n    \"meetingMembers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/MeetingMemberDTO\"\n      }\n    },\n    \"languageId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"passwordProtected\": {\n      \"type\": \"boolean\"\n    },\n    \"connectedEvent\": {\n      \"type\": \"boolean\"\n    },\n    \"reminderEmailSend\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-appointment-dto-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: AppointmentDTO
---
