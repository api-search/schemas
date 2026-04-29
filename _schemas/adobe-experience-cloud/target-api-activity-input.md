---
description: ActivityInput schema
layout: schema
name: ActivityInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: priority
  type: integer
- description: ''
  name: startsAt
  type: string
- description: ''
  name: endsAt
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-activity-input-schema.json
slug: target-api-activity-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-activity-input-schema.json\",\n  \"title\": \"ActivityInput\",\n  \"description\": \"ActivityInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"type\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ab\",\n        \"xt\",\n        \"mvt\",\n        \"ap\"\n      ]\n    },\n    \"priority\": {\n      \"type\": \"integer\"\n    },\n    \"startsAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"endsAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-activity-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ActivityInput
---
