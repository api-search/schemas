---
description: An action plan created to address survey findings
layout: schema
name: ActionPlan
properties_list:
- description: Unique identifier for the action plan
  name: plan_id
  type: string
- description: Survey this action plan relates to
  name: survey_id
  type: string
- description: Title of the action plan
  name: title
  type: string
- description: Detailed description of the planned actions
  name: description
  type: string
- description: Current status of the action plan
  name: status
  type: string
- description: Name of the action plan owner
  name: owner
  type: string
- description: Target completion date for the action plan
  name: due_date
  type: string
- description: Timestamp when the action plan was created
  name: created_at
  type: string
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-action-plan-schema.json
slug: engagement-survey-action-plan
source_filename: engagement-survey-action-plan-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-action-plan-schema.json\",\n  \"title\": \"ActionPlan\",\n  \"description\": \"An action plan created to address survey findings\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"plan_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the action plan\",\n      \"example\": \"plan-500111\"\n    },\n    \"survey_id\": {\n      \"type\": \"string\",\n      \"description\": \"Survey this action plan relates to\",\n      \"example\": \"survey-500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the action plan\",\n      \"example\": \"Improve Manager Communication\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Detailed description of the planned actions\"\
  ,\n      \"example\": \"Increase frequency of team meetings and transparency\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Current status of the action plan\",\n      \"enum\": [\n        \"not_started\",\n        \"in_progress\",\n        \"completed\",\n        \"cancelled\"\n      ],\n      \"example\": \"in_progress\"\n    },\n    \"owner\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the action plan owner\",\n      \"example\": \"Jane Smith\"\n    },\n    \"due_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Target completion date for the action plan\",\n      \"example\": \"2026-09-30\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the action plan was created\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-action-plan-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: ActionPlan
---
