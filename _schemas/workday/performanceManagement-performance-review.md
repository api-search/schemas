---
description: ''
layout: schema
name: PerformanceReview
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: descriptor
  type: string
- description: The review status (e.g., In Progress, Manager Evaluation, Completed).
  name: status
  type: string
- description: ''
  name: completedDate
  type: string
provider_name: Workday
provider_slug: workday
schema_file: json-schema/performanceManagement-performance-review-schema.json
slug: performanceManagement-performance-review
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PerformanceReview\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"descriptor\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The review status (e.g., In Progress, Manager Evaluation, Completed).\"\n    },\n    \"completedDate\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/json-schema/performanceManagement-performance-review-schema.json
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
title: PerformanceReview
---
