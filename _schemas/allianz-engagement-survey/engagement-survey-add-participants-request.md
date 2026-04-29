---
description: Request body to add participants to a survey
layout: schema
name: AddParticipantsRequest
properties_list:
- description: List of employee IDs to add as participants
  name: employee_ids
  type: array
- description: Whether to send invitation emails immediately
  name: send_invitation
  type: boolean
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-add-participants-request-schema.json
slug: engagement-survey-add-participants-request
source_filename: engagement-survey-add-participants-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-add-participants-request-schema.json\",\n  \"title\": \"AddParticipantsRequest\",\n  \"description\": \"Request body to add participants to a survey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"employee_ids\": {\n      \"type\": \"array\",\n      \"description\": \"List of employee IDs to add as participants\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"example\": [\n        \"emp-123456\",\n        \"emp-123457\"\n      ]\n    },\n    \"send_invitation\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to send invitation emails immediately\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"employee_ids\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-add-participants-request-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: AddParticipantsRequest
---
