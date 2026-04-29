---
description: Paginated list of engagement surveys
layout: schema
name: SurveyList
properties_list:
- description: Total number of surveys matching the filter
  name: total
  type: integer
- description: Current pagination offset
  name: offset
  type: integer
- description: Maximum number returned per page
  name: limit
  type: integer
- description: List of survey objects
  name: items
  type: array
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-survey-list-schema.json
slug: engagement-survey-survey-list
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-survey-list-schema.json\",\n  \"title\": \"SurveyList\",\n  \"description\": \"Paginated list of engagement surveys\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of surveys matching the filter\",\n      \"example\": 5\n    },\n    \"offset\": {\n      \"type\": \"integer\",\n      \"description\": \"Current pagination offset\",\n      \"example\": 0\n    },\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum number returned per page\",\n      \"example\": 20\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of survey objects\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/Survey\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-survey-list-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: SurveyList
---
