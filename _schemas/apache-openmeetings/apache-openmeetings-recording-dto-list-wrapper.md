---
description: RecordingDTOListWrapper schema from Apache OpenMeetings REST API
layout: schema
name: RecordingDTOListWrapper
properties_list:
- description: ''
  name: recordingDTO
  type: array
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-recording-dto-list-wrapper-schema.json
slug: apache-openmeetings-recording-dto-list-wrapper
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-recording-dto-list-wrapper-schema.json\",\n  \"title\": \"RecordingDTOListWrapper\",\n  \"description\": \"RecordingDTOListWrapper schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"recordingDTO\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/RecordingDTO\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-recording-dto-list-wrapper-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: RecordingDTOListWrapper
---
