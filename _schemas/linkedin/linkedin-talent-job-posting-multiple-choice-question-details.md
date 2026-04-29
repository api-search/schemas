---
description: MultipleChoiceQuestionDetails from LinkedIn API
layout: schema
name: MultipleChoiceQuestionDetails
properties_list:
- description: ''
  name: choices
  type: array
- description: ''
  name: selectMultiple
  type: boolean
- description: ''
  name: preferredFormComponent
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-multiple-choice-question-details-schema.json
slug: linkedin-talent-job-posting-multiple-choice-question-details
source_filename: linkedin-talent-job-posting-multiple-choice-question-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-multiple-choice-question-details-schema.json\",\n  \"title\": \"MultipleChoiceQuestionDetails\",\n  \"description\": \"MultipleChoiceQuestionDetails from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"choices\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/QuestionChoice\"\n      }\n    },\n    \"selectMultiple\": {\n      \"type\": \"boolean\",\n      \"example\": false\n    },\n    \"preferredFormComponent\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"RADIO_BUTTONS\",\n        \"DROPDOWN\",\n        \"CHECKBOXES\"\n      ],\n      \"example\": \"RADIO_BUTTONS\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-multiple-choice-question-details-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: MultipleChoiceQuestionDetails
---
