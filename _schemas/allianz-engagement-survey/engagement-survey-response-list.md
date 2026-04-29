---
description: Paginated list of anonymized survey responses
layout: schema
name: ResponseList
properties_list:
- description: Total number of responses
  name: total
  type: integer
- description: List of anonymized response records
  name: items
  type: array
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-response-list-schema.json
slug: engagement-survey-response-list
source_filename: engagement-survey-response-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-response-list-schema.json\",\n  \"title\": \"ResponseList\",\n  \"description\": \"Paginated list of anonymized survey responses\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\",\n      \"description\": \"Total number of responses\",\n      \"example\": 876\n    },\n    \"items\": {\n      \"type\": \"array\",\n      \"description\": \"List of anonymized response records\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/SurveyResponse\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-response-list-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: ResponseList
---
