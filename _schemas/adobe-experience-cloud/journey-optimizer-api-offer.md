---
description: Offer schema
layout: schema
name: Offer
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: status
  type: string
- description: ''
  name: representations
  type: array
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
- description: ''
  name: priority
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/journey-optimizer-api-offer-schema.json
slug: journey-optimizer-api-offer
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-offer-schema.json\",\n  \"title\": \"Offer\",\n  \"description\": \"Offer schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"draft\",\n        \"approved\",\n        \"archived\"\n      ]\n    },\n    \"representations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"channel\": {\n            \"type\": \"string\"\n          },\n          \"placement\": {\n            \"type\": \"string\"\n          },\n          \"content\": {\n            \"type\": \"string\"\n          }\n        }\n      }\n    },\n    \"startDate\"\
  : {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"priority\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-offer-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: Offer
---
