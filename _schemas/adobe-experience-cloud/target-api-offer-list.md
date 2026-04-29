---
description: OfferList schema
layout: schema
name: OfferList
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
  name: offers
  type: array
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-offer-list-schema.json
slug: target-api-offer-list
source_filename: target-api-offer-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-offer-list-schema.json\",\n  \"title\": \"OfferList\",\n  \"description\": \"OfferList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"total\": {\n      \"type\": \"integer\"\n    },\n    \"offset\": {\n      \"type\": \"integer\"\n    },\n    \"limit\": {\n      \"type\": \"integer\"\n    },\n    \"offers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"content\",\n              \"redirect\",\n              \"dynamic\"\n            ]\n          },\n          \"content\":\
  \ {\n            \"type\": \"string\"\n          },\n          \"modifiedAt\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          }\n        }\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-offer-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: OfferList
---
