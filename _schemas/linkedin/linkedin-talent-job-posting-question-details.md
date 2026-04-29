---
description: QuestionDetails from LinkedIn API
layout: schema
name: QuestionDetails
properties_list:
- description: ''
  name: multipleChoiceQuestionDetails
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-question-details-schema.json
slug: linkedin-talent-job-posting-question-details
source_filename: linkedin-talent-job-posting-question-details-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-question-details-schema.json\",\n  \"title\": \"QuestionDetails\",\n  \"description\": \"QuestionDetails from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"multipleChoiceQuestionDetails\": {\n      \"$ref\": \"#/components/schemas/MultipleChoiceQuestionDetails\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-question-details-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: QuestionDetails
---
