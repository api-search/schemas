---
description: CoverLetterQuestions from LinkedIn API
layout: schema
name: CoverLetterQuestions
properties_list:
- description: ''
  name: coverLetterQuestionRequirement
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-cover-letter-questions-schema.json
slug: linkedin-talent-job-posting-cover-letter-questions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-cover-letter-questions-schema.json\",\n  \"title\": \"CoverLetterQuestions\",\n  \"description\": \"CoverLetterQuestions from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"coverLetterQuestionRequirement\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"REQUIRED\",\n        \"OPTIONAL\",\n        \"NOT_AVAILABLE\"\n      ],\n      \"example\": \"OPTIONAL\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-cover-letter-questions-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: CoverLetterQuestions
---
