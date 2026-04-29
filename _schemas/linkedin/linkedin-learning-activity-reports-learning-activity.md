---
description: LearningActivity from LinkedIn API
layout: schema
name: LearningActivity
properties_list:
- description: Type of engagement activity
  name: engagementType
  type: string
- description: Numeric value of the engagement
  name: engagementValue
  type: integer
- description: Whether the metric is unique or total count
  name: engagementMetricQualifier
  type: string
- description: Type of learning asset
  name: assetType
  type: string
- description: Timestamp of first engagement
  name: firstEngagedAt
  type: integer
- description: Timestamp of last engagement
  name: lastEngagedAt
  type: integer
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-learning-activity-reports-learning-activity-schema.json
slug: linkedin-learning-activity-reports-learning-activity
source_filename: linkedin-learning-activity-reports-learning-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-learning-activity-schema.json\",\n  \"title\": \"LearningActivity\",\n  \"description\": \"LearningActivity from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"engagementType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"LOGINS\",\n        \"VIEWS\",\n        \"SECONDS_VIEWED\",\n        \"COMPLETIONS\"\n      ],\n      \"description\": \"Type of engagement activity\",\n      \"example\": \"LOGINS\"\n    },\n    \"engagementValue\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric value of the engagement\",\n      \"example\": 88\n    },\n    \"engagementMetricQualifier\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"UNIQUE\",\n        \"TOTAL\"\n      ],\n      \"description\": \"Whether the metric is\
  \ unique or total count\",\n      \"example\": \"UNIQUE\"\n    },\n    \"assetType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"VIDEO\",\n        \"ARTICLE\",\n        \"AUDIO\",\n        \"BOOK\",\n        \"LEARNING_COLLECTION\",\n        \"COURSE\",\n        \"DOCUMENT\",\n        \"EVENT\",\n        \"LEARNING_PATH\"\n      ],\n      \"description\": \"Type of learning asset\",\n      \"example\": \"VIDEO\"\n    },\n    \"firstEngagedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp of first engagement\",\n      \"example\": 1627267600000\n    },\n    \"lastEngagedAt\": {\n      \"type\": \"integer\",\n      \"format\": \"int64\",\n      \"description\": \"Timestamp of last engagement\",\n      \"example\": 1627354000000\n    }\n  },\n  \"required\": [\n    \"engagementType\",\n    \"engagementValue\",\n    \"engagementMetricQualifier\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-learning-activity-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: LearningActivity
---
