---
description: AdditionalQuestions from LinkedIn API
layout: schema
name: AdditionalQuestions
properties_list:
- description: ''
  name: customQuestionSets
  type: array
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-additional-questions-schema.json
slug: linkedin-talent-job-posting-additional-questions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-additional-questions-schema.json\",\n  \"title\": \"AdditionalQuestions\",\n  \"description\": \"AdditionalQuestions from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"customQuestionSets\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/CustomQuestionSet\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-additional-questions-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: AdditionalQuestions
---
