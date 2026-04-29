---
description: ActivityList schema
layout: schema
name: ActivityList
properties_list:
- description: ''
  name: total
  type: integer
- description: ''
  name: offset
  type: integer
- description: ''
  name: limit
  type: integer
- description: ''
  name: activities
  type: array
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-activity-list-schema.json
slug: target-api-activity-list
source_filename: target-api-activity-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-activity-list-schema.json\",\n  \"title\": \"ActivityList\",\n  \"description\": \"ActivityList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"activities\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"ab\",\n              \"xt\",\n              \"mvt\",\n              \"ap\"\n            ]\n          },\n \
  \         \"state\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"approved\",\n              \"deactivated\",\n              \"archived\"\n            ]\n          },\n          \"priority\": {\n            \"type\": \"integer\"\n          },\n          \"modifiedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"startsAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"endsAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-activity-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ActivityList
---
