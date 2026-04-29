---
description: CustomQuestion from LinkedIn API
layout: schema
name: CustomQuestion
properties_list:
- description: ''
  name: required
  type: boolean
- description: ''
  name: partnerQuestionIdentifier
  type: string
- description: ''
  name: questionText
  type: string
- description: ''
  name: questionDetails
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-custom-question-schema.json
slug: linkedin-talent-job-posting-custom-question
source_filename: linkedin-talent-job-posting-custom-question-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-custom-question-schema.json\",\n  \"title\": \"CustomQuestion\",\n  \"description\": \"CustomQuestion from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"required\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"partnerQuestionIdentifier\": {\n      \"type\": \"string\",\n      \"example\": \"question-001\"\n    },\n    \"questionText\": {\n      \"type\": \"string\",\n      \"example\": \"Are you authorized to work in the United States?\"\n    },\n    \"questionDetails\": {\n      \"$ref\": \"#/components/schemas/QuestionDetails\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-custom-question-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CustomQuestion
---
