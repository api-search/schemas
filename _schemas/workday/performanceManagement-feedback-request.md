---
description: ''
layout: schema
name: FeedbackRequest
properties_list:
- description: ''
  name: respondents
  type: array
- description: ''
  name: questions
  type: array
- description: ''
  name: dueDate
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/performanceManagement-feedback-request-schema.json
slug: performanceManagement-feedback-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FeedbackRequest\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"respondents\": {\n      \"type\": \"array\"\n    },\n    \"questions\": {\n      \"type\": \"array\"\n    },\n    \"dueDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/performanceManagement-feedback-request-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: FeedbackRequest
---
