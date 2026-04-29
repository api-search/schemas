---
description: A survey participant record
layout: schema
name: Participant
properties_list:
- description: Unique identifier for the participant record
  name: participant_id
  type: string
- description: Allianz employee identifier
  name: employee_id
  type: string
- description: Current response status of the participant
  name: status
  type: string
- description: Timestamp when the invitation was sent
  name: invited_at
  type: string
- description: Timestamp when the participant submitted their response
  name: responded_at
  type: string
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-participant-schema.json
slug: engagement-survey-participant
source_filename: engagement-survey-participant-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-participant-schema.json\",\n  \"title\": \"Participant\",\n  \"description\": \"A survey participant record\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"participant_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the participant record\",\n      \"example\": \"part-500456\"\n    },\n    \"employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Allianz employee identifier\",\n      \"example\": \"emp-123456\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current response status of the participant\",\n      \"enum\": [\n        \"invited\",\n        \"responded\",\n        \"not_responded\"\n      ],\n      \"example\": \"responded\"\n    },\n    \"invited_at\": {\n      \"type\"\
  : \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the invitation was sent\",\n      \"example\": \"2026-05-01T08:00:00Z\"\n    },\n    \"responded_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the participant submitted their response\",\n      \"example\": \"2026-05-03T14:22:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-participant-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: Participant
---
