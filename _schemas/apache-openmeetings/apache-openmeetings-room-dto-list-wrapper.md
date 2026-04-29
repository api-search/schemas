---
description: RoomDTOListWrapper schema from Apache OpenMeetings REST API
layout: schema
name: RoomDTOListWrapper
properties_list:
- description: ''
  name: roomDTO
  type: array
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-room-dto-list-wrapper-schema.json
slug: apache-openmeetings-room-dto-list-wrapper
source_filename: apache-openmeetings-room-dto-list-wrapper-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-room-dto-list-wrapper-schema.json\",\n  \"title\": \"RoomDTOListWrapper\",\n  \"description\": \"RoomDTOListWrapper schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"roomDTO\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RoomDTO\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-room-dto-list-wrapper-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: RoomDTOListWrapper
---
