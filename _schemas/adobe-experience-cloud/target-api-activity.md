---
description: Activity schema
layout: schema
name: Activity
properties_list:
- description: ''
  name: id
  type: integer
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: priority
  type: integer
- description: ''
  name: modifiedAt
  type: string
- description: ''
  name: startsAt
  type: string
- description: ''
  name: endsAt
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-activity-schema.json
slug: target-api-activity
source_filename: target-api-activity-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-activity-schema.json\",\n  \"title\": \"Activity\",\n  \"description\": \"Activity schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"integer\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"ab\",\n        \"xt\",\n        \"mvt\",\n        \"ap\"\n      ]\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"approved\",\n        \"deactivated\",\n        \"archived\"\n      ]\n    },\n    \"priority\": {\n      \"type\": \"integer\"\n    },\n    \"modifiedAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"startsAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n   \
  \ \"endsAt\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-activity-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Activity
---
