---
description: ResumeQuestions from LinkedIn API
layout: schema
name: ResumeQuestions
properties_list:
- description: ''
  name: resumeQuestionRequirement
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-resume-questions-schema.json
slug: linkedin-talent-job-posting-resume-questions
source_filename: linkedin-talent-job-posting-resume-questions-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-resume-questions-schema.json\",\n  \"title\": \"ResumeQuestions\",\n  \"description\": \"ResumeQuestions from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resumeQuestionRequirement\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"REQUIRED\",\n        \"OPTIONAL\",\n        \"NOT_AVAILABLE\"\n      ],\n      \"example\": \"REQUIRED\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-resume-questions-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ResumeQuestions
---
