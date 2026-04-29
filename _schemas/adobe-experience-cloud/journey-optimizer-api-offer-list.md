---
description: OfferList schema
layout: schema
name: OfferList
properties_list:
- description: ''
  name: offers
  type: array
- description: ''
  name: totalCount
  type: integer
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/journey-optimizer-api-offer-list-schema.json
slug: journey-optimizer-api-offer-list
source_filename: journey-optimizer-api-offer-list-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-offer-list-schema.json\",\n  \"title\": \"OfferList\",\n  \"description\": \"OfferList schema\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"offers\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"string\"\n          },\n          \"name\": {\n            \"type\": \"string\"\n          },\n          \"status\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"draft\",\n              \"approved\",\n              \"archived\"\n            ]\n          },\n          \"representations\": {\n            \"type\": \"array\",\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n             \
  \   \"channel\": {\n                  \"type\": \"string\"\n                },\n                \"placement\": {\n                  \"type\": \"string\"\n                },\n                \"content\": {\n                  \"type\": \"string\"\n                }\n              }\n            }\n          },\n          \"startDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"endDate\": {\n            \"type\": \"string\",\n            \"format\": \"date-time\"\n          },\n          \"priority\": {\n            \"type\": \"integer\"\n          }\n        }\n      }\n    },\n    \"totalCount\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-offer-list-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: OfferList
---
