---
description: A question in a Google Form.
layout: schema
name: Question
properties_list:
- description: Output only. The ID of the question.
  name: questionId
  type: string
- description: Whether the question must be answered.
  name: required
  type: boolean
- description: ''
  name: grading
  type: object
- description: ''
  name: choiceQuestion
  type: object
- description: ''
  name: textQuestion
  type: object
- description: ''
  name: scaleQuestion
  type: object
- description: ''
  name: dateQuestion
  type: object
- description: ''
  name: timeQuestion
  type: object
provider_name: Google Forms
provider_slug: google-forms
schema_file: json-schema/google-forms-api-question-schema.json
slug: google-forms-api-question
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/json-schema/google-forms-api-question-schema.json\",\n  \"title\": \"Question\",\n  \"description\": \"A question in a Google Form.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"questionId\": { \"type\": \"string\", \"description\": \"Output only. The ID of the question.\", \"readOnly\": true },\n    \"required\": { \"type\": \"boolean\", \"description\": \"Whether the question must be answered.\" },\n    \"grading\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"pointValue\": { \"type\": \"integer\", \"description\": \"Points available for this question.\" },\n        \"correctAnswers\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"answers\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"object\",\n    \
  \            \"properties\": {\n                  \"value\": { \"type\": \"string\" }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"choiceQuestion\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": { \"type\": \"string\", \"enum\": [\"CHOICE_TYPE_UNSPECIFIED\", \"RADIO\", \"CHECKBOX\", \"DROP_DOWN\"] },\n        \"options\": {\n          \"type\": \"array\",\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"value\": { \"type\": \"string\" },\n              \"isOther\": { \"type\": \"boolean\" }\n            }\n          }\n        },\n        \"shuffle\": { \"type\": \"boolean\" }\n      }\n    },\n    \"textQuestion\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"paragraph\": { \"type\": \"boolean\", \"description\": \"Whether the question accepts paragraph text.\" }\n      }\n    },\n    \"scaleQuestion\": {\n      \"type\": \"\
  object\",\n      \"properties\": {\n        \"low\": { \"type\": \"integer\" },\n        \"high\": { \"type\": \"integer\" },\n        \"lowLabel\": { \"type\": \"string\" },\n        \"highLabel\": { \"type\": \"string\" }\n      }\n    },\n    \"dateQuestion\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"includeTime\": { \"type\": \"boolean\" },\n        \"includeYear\": { \"type\": \"boolean\" }\n      }\n    },\n    \"timeQuestion\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"duration\": { \"type\": \"boolean\" }\n      }\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/json-schema/google-forms-api-question-schema.json
tags:
- Data Collection
- Forms
- Google
- Google Workspace
- Questionnaires
- Responses
- Surveys
title: Question
---
