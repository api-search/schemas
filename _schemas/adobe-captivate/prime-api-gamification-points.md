---
description: Gamification points for a user
layout: schema
name: GamificationPoints
properties_list:
- description: Unique identifier
  name: id
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: attributes
  type: object
provider_name: Adobe Captivate
provider_slug: adobe-captivate
schema_file: json-schema/prime-api-gamification-points-schema.json
slug: prime-api-gamification-points
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-gamification-points-schema.json\",\n  \"title\": \"GamificationPoints\",\n  \"description\": \"Gamification points for a user\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"const\": \"gamification\"\n    },\n    \"attributes\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"learnerPoints\": {\n          \"type\": \"integer\",\n          \"description\": \"Points earned through learning activities\"\n        },\n        \"managerPoints\": {\n          \"type\": \"integer\",\n          \"description\": \"Points earned as a manager\"\n        },\n        \"overallPoints\": {\n          \"type\": \"integer\",\n          \"description\"\
  : \"Total points across all categories\"\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-captivate/refs/heads/main/json-schema/prime-api-gamification-points-schema.json
tags:
- Authoring
- Education
- eLearning
- LMS
- SCORM
- Training
- xAPI
title: GamificationPoints
---
