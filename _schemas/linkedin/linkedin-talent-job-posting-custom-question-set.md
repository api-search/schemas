---
description: CustomQuestionSet from LinkedIn API
layout: schema
name: CustomQuestionSet
properties_list:
- description: ''
  name: questionSetId
  type: string
- description: ''
  name: questions
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-custom-question-set-schema.json
slug: linkedin-talent-job-posting-custom-question-set
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-custom-question-set-schema.json\",\n  \"title\": \"CustomQuestionSet\",\n  \"description\": \"CustomQuestionSet from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"questionSetId\": {\n      \"type\": \"string\",\n      \"example\": \"custom-questions-001\"\n    },\n    \"questions\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CustomQuestion\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-custom-question-set-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CustomQuestionSet
---
