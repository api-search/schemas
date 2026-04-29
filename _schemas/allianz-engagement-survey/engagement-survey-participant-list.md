---
description: List of survey participants with participation statistics
layout: schema
name: ParticipantList
properties_list:
- description: Total number of invited participants
  name: total
  type: integer
- description: Number of participants who responded
  name: responded
  type: integer
- description: Percentage of participants who responded
  name: participation_rate
  type: number
- description: List of participant records
  name: items
  type: array
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-participant-list-schema.json
slug: engagement-survey-participant-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-participant-list-schema.json\",\n  \"title\": \"ParticipantList\",\n  \"description\": \"List of survey participants with participation statistics\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of invited participants\",\n      \"example\": 1250\n    },\n    \"responded\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of participants who responded\",\n      \"example\": 876\n    },\n    \"participation_rate\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Percentage of participants who responded\",\n      \"example\": 70.1\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of participant records\"\
  ,\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Participant\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-participant-list-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: ParticipantList
---
