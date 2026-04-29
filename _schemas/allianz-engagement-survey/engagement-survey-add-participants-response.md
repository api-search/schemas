---
description: Result of adding participants to a survey
layout: schema
name: AddParticipantsResponse
properties_list:
- description: Number of participants successfully added
  name: added
  type: integer
- description: Whether invitation emails were sent
  name: invitation_sent
  type: boolean
- description: Number of employees that could not be added
  name: failed
  type: integer
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-add-participants-response-schema.json
slug: engagement-survey-add-participants-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-add-participants-response-schema.json\",\n  \"title\": \"AddParticipantsResponse\",\n  \"description\": \"Result of adding participants to a survey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"added\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of participants successfully added\",\n      \"example\": 2\n    },\n    \"invitation_sent\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether invitation emails were sent\",\n      \"example\": true\n    },\n    \"failed\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of employees that could not be added\",\n      \"example\": 0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-add-participants-response-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: AddParticipantsResponse
---
