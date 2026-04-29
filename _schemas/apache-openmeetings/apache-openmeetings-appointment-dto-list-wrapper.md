---
description: AppointmentDTOListWrapper schema from Apache OpenMeetings REST API
layout: schema
name: AppointmentDTOListWrapper
properties_list:
- description: ''
  name: appointmentDTO
  type: array
provider_name: Apache OpenMeetings
provider_slug: apache-openmeetings
schema_file: json-schema/apache-openmeetings-appointment-dto-list-wrapper-schema.json
slug: apache-openmeetings-appointment-dto-list-wrapper
source_filename: apache-openmeetings-appointment-dto-list-wrapper-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-appointment-dto-list-wrapper-schema.json\",\n  \"title\": \"AppointmentDTOListWrapper\",\n  \"description\": \"AppointmentDTOListWrapper schema from Apache OpenMeetings REST API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"appointmentDTO\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/AppointmentDTO\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-openmeetings/refs/heads/main/json-schema/apache-openmeetings-appointment-dto-list-wrapper-schema.json
tags:
- Collaboration
- Video Conferencing
- Web Conferencing
- Whiteboard
- Apache
- Open Source
- Conferencing
title: AppointmentDTOListWrapper
---
