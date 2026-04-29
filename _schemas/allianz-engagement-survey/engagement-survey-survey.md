---
description: An employee engagement survey definition
layout: schema
name: Survey
properties_list:
- description: Unique identifier for the survey
  name: survey_id
  type: string
- description: Title of the survey
  name: title
  type: string
- description: Type of engagement survey
  name: survey_type
  type: string
- description: Current lifecycle status of the survey
  name: status
  type: string
- description: Description of the survey purpose and scope
  name: description
  type: string
- description: Date when the survey becomes available to participants
  name: start_date
  type: string
- description: Date when the survey closes
  name: end_date
  type: string
- description: Timestamp when the survey was created
  name: created_at
  type: string
- description: Timestamp when the survey was last modified
  name: modified_at
  type: string
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-survey-schema.json
slug: engagement-survey-survey
source_filename: engagement-survey-survey-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-survey-schema.json\",\n  \"title\": \"Survey\",\n  \"description\": \"An employee engagement survey definition\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"survey_id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the survey\",\n      \"example\": \"survey-500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"description\": \"Title of the survey\",\n      \"example\": \"2026 Global Engagement Survey\"\n    },\n    \"survey_type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of engagement survey\",\n      \"enum\": [\n        \"annual\",\n        \"pulse\",\n        \"onboarding\",\n        \"exit\"\n      ],\n      \"example\": \"annual\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n\
  \      \"description\": \"Current lifecycle status of the survey\",\n      \"enum\": [\n        \"draft\",\n        \"active\",\n        \"closed\",\n        \"archived\"\n      ],\n      \"example\": \"active\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the survey purpose and scope\",\n      \"example\": \"Annual employee engagement measurement for all Allianz entities\"\n    },\n    \"start_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the survey becomes available to participants\",\n      \"example\": \"2026-05-01\"\n    },\n    \"end_date\": {\n      \"type\": \"string\",\n      \"format\": \"date\",\n      \"description\": \"Date when the survey closes\",\n      \"example\": \"2026-05-31\"\n    },\n    \"created_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the survey was created\",\n      \"example\"\
  : \"2026-04-19T10:00:00Z\"\n    },\n    \"modified_at\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Timestamp when the survey was last modified\",\n      \"example\": \"2026-04-19T10:00:00Z\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-survey-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: Survey
---
