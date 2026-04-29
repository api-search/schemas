---
description: A response to a Google Form.
layout: schema
name: FormResponse
properties_list:
- description: Output only. The form ID.
  name: formId
  type: string
- description: Output only. The response ID.
  name: responseId
  type: string
- description: Timestamp for the first time the response was submitted.
  name: createTime
  type: string
- description: Timestamp for the most recent submission.
  name: lastSubmittedTime
  type: string
- description: The email address of the respondent.
  name: respondentEmail
  type: string
- description: The actual answers keyed by question ID.
  name: answers
  type: object
- description: Total points awarded for quiz forms.
  name: totalScore
  type: number
provider_name: Google Forms
provider_slug: google-forms
schema_file: json-schema/google-forms-api-form-response-schema.json
slug: google-forms-api-form-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/json-schema/google-forms-api-form-response-schema.json\",\n  \"title\": \"FormResponse\",\n  \"description\": \"A response to a Google Form.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"formId\": { \"type\": \"string\", \"description\": \"Output only. The form ID.\", \"readOnly\": true },\n    \"responseId\": { \"type\": \"string\", \"description\": \"Output only. The response ID.\", \"readOnly\": true },\n    \"createTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp for the first time the response was submitted.\" },\n    \"lastSubmittedTime\": { \"type\": \"string\", \"format\": \"date-time\", \"description\": \"Timestamp for the most recent submission.\" },\n    \"respondentEmail\": { \"type\": \"string\", \"format\": \"email\", \"description\": \"The email address\
  \ of the respondent.\" },\n    \"answers\": {\n      \"type\": \"object\",\n      \"description\": \"The actual answers keyed by question ID.\",\n      \"additionalProperties\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"questionId\": { \"type\": \"string\" },\n          \"textAnswers\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"answers\": {\n                \"type\": \"array\",\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"value\": { \"type\": \"string\" }\n                  }\n                }\n              }\n            }\n          }\n        }\n      }\n    },\n    \"totalScore\": { \"type\": \"number\", \"description\": \"Total points awarded for quiz forms.\" }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/google-forms/refs/heads/main/json-schema/google-forms-api-form-response-schema.json
tags:
- Data Collection
- Forms
- Google
- Google Workspace
- Questionnaires
- Responses
- Surveys
title: FormResponse
---
