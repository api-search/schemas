---
description: InvitationDTO schema from Apache OpenMeetings REST API
layout: schema
name: InvitationDTO
properties_list:
- description: ''
  name: email
  type: string
- description: ''
  name: firstname
  type: string
- description: ''
  name: lastname
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: subject
  type: string
- description: ''
  name: roomId
  type: integer
- description: ''
  name: passwordProtected
  type: boolean
- description: ''
  name: password
  type: string
- description: ''
  name: valid
  type: string
- description: ''
  name: validFrom
  type: string
- description: ''
  name: validTo
  type: string
- description: ''
  name: languageId
  type: integer
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-invitation-dto-schema.json
slug: apache-openmeetings-invitation-dto
source_filename: apache-openmeetings-invitation-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-invitation-dto-schema.json\",\n  \"title\": \"InvitationDTO\",\n  \"description\": \"InvitationDTO schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"email\": {\n      \"type\": \"string\"\n    },\n    \"firstname\": {\n      \"type\": \"string\"\n    },\n    \"lastname\": {\n      \"type\": \"string\"\n    },\n    \"message\": {\n      \"type\": \"string\"\n    },\n    \"subject\": {\n      \"type\": \"string\"\n    },\n    \"roomId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"passwordProtected\": {\n      \"type\": \"boolean\"\n    },\n    \"password\": {\n      \"type\": \"string\"\n    },\n    \"valid\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ONE_TIME\",\n        \"PERIOD\"\
  ,\n        \"ENDLESS\"\n      ]\n    },\n    \"validFrom\": {\n      \"type\": \"string\"\n    },\n    \"validTo\": {\n      \"type\": \"string\"\n    },\n    \"languageId\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-invitation-dto-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: InvitationDTO
---
