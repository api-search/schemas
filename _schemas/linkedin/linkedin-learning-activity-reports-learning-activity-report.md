---
description: LearningActivityReport from LinkedIn API
layout: schema
name: LearningActivityReport
properties_list:
- description: Timestamp of the latest data included in this report
  name: latestDataAt
  type: integer
- description: ''
  name: activities
  type: array
- description: ''
  name: learnerDetails
  type: object
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-learning-activity-reports-learning-activity-report-schema.json
slug: linkedin-learning-activity-reports-learning-activity-report
source_filename: linkedin-learning-activity-reports-learning-activity-report-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-learning-activity-report-schema.json\",\n  \"title\": \"LearningActivityReport\",\n  \"description\": \"LearningActivityReport from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"latestDataAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp of the latest data included in this report\",\n      \"example\": 1632207540000\n    },\n    \"activities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/LearningActivity\"\n      }\n    },\n    \"learnerDetails\": {\n      \"$ref\": \"#/components/schemas/LearnerDetails\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-learning-activity-report-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: LearningActivityReport
---
