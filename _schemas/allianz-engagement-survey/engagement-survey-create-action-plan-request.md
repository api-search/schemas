---
description: Request body for creating a new action plan
layout: schema
name: CreateActionPlanRequest
properties_list:
- description: Title of the action plan
  name: title
  type: string
- description: Description of planned actions
  name: description
  type: string
- description: Employee ID of the action plan owner
  name: owner_employee_id
  type: string
- description: Target completion date
  name: due_date
  type: string
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-create-action-plan-request-schema.json
slug: engagement-survey-create-action-plan-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-create-action-plan-request-schema.json\",\n  \"title\": \"CreateActionPlanRequest\",\n  \"description\": \"Request body for creating a new action plan\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the action plan\",\n      \"example\": \"Improve Manager Communication\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of planned actions\",\n      \"example\": \"Increase frequency of team meetings and transparency\"\n    },\n    \"owner_employee_id\": {\n      \"type\": \"string\",\n      \"description\": \"Employee ID of the action plan owner\",\n      \"example\": \"emp-123456\"\n    },\n    \"due_date\": {\n      \"type\": \"string\",\n    \
  \  \"format\": \"date\",\n      \"description\": \"Target completion date\",\n      \"example\": \"2026-09-30\"\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"owner_employee_id\",\n    \"due_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-create-action-plan-request-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: CreateActionPlanRequest
---
