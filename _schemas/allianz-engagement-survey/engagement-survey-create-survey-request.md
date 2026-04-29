---
description: Request body for creating a new engagement survey
layout: schema
name: CreateSurveyRequest
properties_list:
- description: Title of the survey
  name: title
  type: string
- description: Type of the survey
  name: survey_type
  type: string
- description: Survey purpose and scope description
  name: description
  type: string
- description: Survey open date
  name: start_date
  type: string
- description: Survey close date
  name: end_date
  type: string
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-create-survey-request-schema.json
slug: engagement-survey-create-survey-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-create-survey-request-schema.json\",\n  \"title\": \"CreateSurveyRequest\",\n  \"description\": \"Request body for creating a new engagement survey\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the survey\",\n      \"example\": \"2026 Global Engagement Survey\"\n    },\n    \"survey_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the survey\",\n      \"enum\": [\n        \"annual\",\n        \"pulse\",\n        \"onboarding\",\n        \"exit\"\n      ],\n      \"example\": \"annual\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Survey purpose and scope description\",\n      \"example\": \"Annual employee engagement measurement\"\
  \n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Survey open date\",\n      \"example\": \"2026-05-01\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Survey close date\",\n      \"example\": \"2026-05-31\"\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"survey_type\",\n    \"start_date\",\n    \"end_date\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-create-survey-request-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: CreateSurveyRequest
---
