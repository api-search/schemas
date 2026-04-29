---
description: Score summary for a single survey question
layout: schema
name: QuestionScore
properties_list:
- description: Question identifier
  name: question_id
  type: string
- description: The survey question text
  name: question
  type: string
- description: Average score on a 1-5 scale
  name: score
  type: number
- description: Percentage of favorable responses (4-5 on Likert scale)
  name: favorable
  type: number
provider_name: Allianz Engagement Survey
provider_slug: allianz-engagement-survey
schema_file: json-schema/engagement-survey-question-score-schema.json
slug: engagement-survey-question-score
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-question-score-schema.json\",\n  \"title\": \"QuestionScore\",\n  \"description\": \"Score summary for a single survey question\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"question_id\": {\n      \"type\": \"string\",\n      \"description\": \"Question identifier\",\n      \"example\": \"q-001\"\n    },\n    \"question\": {\n      \"type\": \"string\",\n      \"description\": \"The survey question text\",\n      \"example\": \"I am proud to work for Allianz\"\n    },\n    \"score\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Average score on a 1-5 scale\",\n      \"example\": 4.2\n    },\n    \"favorable\": {\n      \"type\": \"number\",\n      \"format\": \"double\",\n      \"description\": \"Percentage of favorable responses\
  \ (4-5 on Likert scale)\",\n      \"example\": 84.0\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/allianz-engagement-survey/refs/heads/main/json-schema/engagement-survey-question-score-schema.json
tags:
- Analytics
- Enterprise
- Human Resources
- Insurance
- Surveys
- Employee Experience
title: QuestionScore
---
