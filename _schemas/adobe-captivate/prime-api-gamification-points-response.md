---
description: User gamification points response
layout: schema
name: GamificationPointsResponse
properties_list:
- description: Gamification points for a user
  name: data
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-gamification-points-response-schema.json
slug: prime-api-gamification-points-response
source_filename: prime-api-gamification-points-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-gamification-points-response-schema.json\",\n  \"title\": \"GamificationPointsResponse\",\n  \"description\": \"User gamification points response\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"description\": \"Gamification points for a user\",\n      \"properties\": {\n        \"id\": {\n          \"type\": \"string\",\n          \"description\": \"Unique identifier\"\n        },\n        \"type\": {\n          \"type\": \"string\",\n          \"const\": \"gamification\"\n        },\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"learnerPoints\": {\n              \"type\": \"integer\",\n              \"description\": \"Points earned through learning activities\"\n            },\n \
  \           \"managerPoints\": {\n              \"type\": \"integer\",\n              \"description\": \"Points earned as a manager\"\n            },\n            \"overallPoints\": {\n              \"type\": \"integer\",\n              \"description\": \"Total points across all categories\"\n            }\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-gamification-points-response-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: GamificationPointsResponse
---
