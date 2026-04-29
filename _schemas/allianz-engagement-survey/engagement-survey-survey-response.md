---
description: An anonymized survey response submission
layout: schema
name: SurveyResponse
properties_list:
- description: Unique identifier for the response
  name: response_id
  type: string
- description: Survey this response belongs to
  name: survey_id
  type: string
- description: Timestamp when the response was submitted
  name: submitted_at
  type: string
- description: List of question answers
  name: answers
  type: array
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-survey-response-schema.json
slug: engagement-survey-survey-response
source_filename: engagement-survey-survey-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-survey-response-schema.json\",\n  \"title\": \"SurveyResponse\",\n  \"description\": \"An anonymized survey response submission\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"response_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the response\",\n      \"example\": \"resp-500789\"\n    },\n    \"survey_id\": {\n      \"type\": \"string\",\n      \"description\": \"Survey this response belongs to\",\n      \"example\": \"survey-500123\"\n    },\n    \"submitted_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the response was submitted\",\n      \"example\": \"2026-05-03T14:22:00Z\"\n    },\n    \"answers\": {\n      \"type\": \"array\",\n      \"description\": \"List\
  \ of question answers\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Answer\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-survey-response-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: SurveyResponse
---
