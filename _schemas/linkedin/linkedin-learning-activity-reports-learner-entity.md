---
description: LearnerEntity from LinkedIn API
layout: schema
name: LearnerEntity
properties_list:
- description: URN of the enterprise account
  name: accountUrn
  type: string
- description: URN of the learner group (if grouped by group)
  name: groupUrn
  type: string
- description: URN of the individual learner (if grouped by individual)
  name: learnerUrn
  type: string
- description: URN of the content (if grouped by content)
  name: contentUrn
  type: string
provider_name: LinkedIn
provider_slug: linkedin
schema_file: json-schema/linkedin-learning-activity-reports-learner-entity-schema.json
slug: linkedin-learning-activity-reports-learner-entity
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-learner-entity-schema.json\",\n  \"title\": \"LearnerEntity\",\n  \"description\": \"LearnerEntity from LinkedIn API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accountUrn\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the enterprise account\",\n      \"example\": \"urn:li:enterpriseAccount:999\"\n    },\n    \"groupUrn\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the learner group (if grouped by group)\",\n      \"example\": \"urn:li:learnerGroup:456\"\n    },\n    \"learnerUrn\": {\n      \"type\": \"string\",\n      \"description\": \"URN of the individual learner (if grouped by individual)\",\n      \"example\": \"urn:li:learner:789\"\n    },\n    \"contentUrn\": {\n      \"type\": \"string\",\n      \"description\":\
  \ \"URN of the content (if grouped by content)\",\n      \"example\": \"urn:li:learningCourse:123\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/linkedin/refs/heads/main/json-schema/linkedin-learning-activity-reports-learner-entity-schema.json
tags:
- Business
- Careers
- Marketing
- Professional Networking
- Recruiting
- Social Media
title: LearnerEntity
---
