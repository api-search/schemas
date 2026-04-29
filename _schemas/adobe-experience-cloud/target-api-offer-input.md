---
description: OfferInput schema
layout: schema
name: OfferInput
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: content
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/target-api-offer-input-schema.json
slug: target-api-offer-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-offer-input-schema.json\",\n  \"title\": \"OfferInput\",\n  \"description\": \"OfferInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"name\",\n    \"type\",\n    \"content\"\n  ],\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"content\",\n        \"redirect\"\n      ]\n    },\n    \"content\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/target-api-offer-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: OfferInput
---
