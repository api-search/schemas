---
description: LearningActivityReportResponse from LinkedIn API
layout: schema
name: LearningActivityReportResponse
properties_list:
- description: ''
  name: elements
  type: array
- description: ''
  name: paging
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-learning-activity-reports-learning-activity-report-response-schema.json
slug: linkedin-learning-activity-reports-learning-activity-report-response
source_filename: linkedin-learning-activity-reports-learning-activity-report-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-learning-activity-report-response-schema.json\",\n  \"title\": \"LearningActivityReportResponse\",\n  \"description\": \"LearningActivityReportResponse from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"elements\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LearningActivityReport\"\n      }\n    },\n    \"paging\": {\n      \"$ref\": \"#/components/schemas/Paging\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-learning-activity-report-response-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: LearningActivityReportResponse
---
