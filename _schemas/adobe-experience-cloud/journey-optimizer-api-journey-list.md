---
description: JourneyList schema
layout: schema
name: JourneyList
properties_list:
- description: ''
  name: journeys
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/journey-optimizer-api-journey-list-schema.json
slug: journey-optimizer-api-journey-list
source_filename: journey-optimizer-api-journey-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-journey-list-schema.json\",\n  \"title\": \"JourneyList\",\n  \"description\": \"JourneyList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"journeys\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"description\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"draft\",\n              \"live\",\n              \"stopped\",\n              \"closed\"\n            ]\n          },\n          \"version\": {\n            \"type\": \"string\"\n         \
  \ },\n          \"createdAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"modifiedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-journey-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: JourneyList
---
