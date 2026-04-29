---
description: OfferInput schema
layout: schema
name: OfferInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: representations
  type: array
- description: ''
  name: eligibilityRule
  type: string
- description: ''
  name: priority
  type: integer
- description: ''
  name: startDate
  type: string
- description: ''
  name: endDate
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/journey-optimizer-api-offer-input-schema.json
slug: journey-optimizer-api-offer-input
source_filename: journey-optimizer-api-offer-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-offer-input-schema.json\",\n  \"title\": \"OfferInput\",\n  \"description\": \"OfferInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"representations\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\"\n      }\n    },\n    \"eligibilityRule\": {\n      \"type\": \"string\"\n    },\n    \"priority\": {\n      \"type\": \"integer\"\n    },\n    \"startDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    },\n    \"endDate\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/journey-optimizer-api-offer-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: OfferInput
---
