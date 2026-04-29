---
description: MeetingMemberDTO schema from Apache OpenMeetings REST API
layout: schema
name: MeetingMemberDTO
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: user
  type: object
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-meeting-member-dto-schema.json
slug: apache-openmeetings-meeting-member-dto
source_filename: apache-openmeetings-meeting-member-dto-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-meeting-member-dto-schema.json\",\n  \"title\": \"MeetingMemberDTO\",\n  \"description\": \"MeetingMemberDTO schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\"\n    },\n    \"user\": {\n      \"$ref\": \"#/components/schemas/UserDTO\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-meeting-member-dto-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: MeetingMemberDTO
---
