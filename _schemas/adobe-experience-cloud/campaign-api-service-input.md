---
description: ServiceInput schema
layout: schema
name: ServiceInput
properties_list:
- description: ''
  name: label
  type: string
- description: ''
  name: name
  type: string
- description: ''
  name: messageType
  type: string
provider_name: Adobe Experience Cloud
provider_slug: adobe-experience-cloud
schema_file: json-schema/campaign-api-service-input-schema.json
slug: campaign-api-service-input
source_filename: campaign-api-service-input-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-service-input-schema.json\",\n  \"title\": \"ServiceInput\",\n  \"description\": \"ServiceInput schema\",\n  \"type\": \"object\",\n  \"required\": [\n    \"label\"\n  ],\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"messageType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"email\",\n        \"sms\"\n      ]\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-experience-cloud/refs/heads/main/json-schema/campaign-api-service-input-schema.json
tags:
- Analytics
- Customer Experience
- Digital Marketing
- Personalization
- Campaign Management
- Journey Orchestration
title: ServiceInput
---
