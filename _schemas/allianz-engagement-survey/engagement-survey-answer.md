---
description: An individual question answer within a survey response
layout: schema
name: Answer
properties_list:
- description: Identifier of the question being answered
  name: question_id
  type: string
- description: Numeric score on a 1-5 Likert scale
  name: score
  type: integer
- description: Open text response for free-text questions
  name: text_response
  type: string
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-answer-schema.json
slug: engagement-survey-answer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-answer-schema.json\",\n  \"title\": \"Answer\",\n  \"description\": \"An individual question answer within a survey response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"question_id\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the question being answered\",\n      \"example\": \"q-001\"\n    },\n    \"score\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric score on a 1-5 Likert scale\",\n      \"minimum\": 1,\n      \"maximum\": 5,\n      \"example\": 4\n    },\n    \"text_response\": {\n      \"type\": \"string\",\n      \"description\": \"Open text response for free-text questions\",\n      \"example\": \"The team culture is very collaborative\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-answer-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: Answer
---
