---
description: Questions configuration for job applications
layout: schema
name: ApplicationQuestions
properties_list:
- description: ''
  name: resumeQuestions
  type: object
- description: ''
  name: coverLetterQuestions
  type: object
- description: Voluntary self-identification questions
  name: voluntarySelfIdentificationQuestions
  type: object
- description: ''
  name: educationQuestions
  type: object
- description: ''
  name: workQuestions
  type: object
- description: ''
  name: additionalQuestions
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-talent-job-posting-application-questions-schema.json
slug: linkedin-talent-job-posting-application-questions
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-application-questions-schema.json\",\n  \"title\": \"ApplicationQuestions\",\n  \"description\": \"Questions configuration for job applications\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resumeQuestions\": {\n      \"$ref\": \"#/components/schemas/ResumeQuestions\"\n    },\n    \"coverLetterQuestions\": {\n      \"$ref\": \"#/components/schemas/CoverLetterQuestions\"\n    },\n    \"voluntarySelfIdentificationQuestions\": {\n      \"type\": \"object\",\n      \"description\": \"Voluntary self-identification questions\"\n    },\n    \"educationQuestions\": {\n      \"$ref\": \"#/components/schemas/EducationQuestions\"\n    },\n    \"workQuestions\": {\n      \"$ref\": \"#/components/schemas/WorkQuestions\"\n    },\n    \"additionalQuestions\": {\n      \"$ref\": \"#/components/schemas/AdditionalQuestions\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-talent-job-posting-application-questions-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: ApplicationQuestions
---
