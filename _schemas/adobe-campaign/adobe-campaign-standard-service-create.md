---
description: ServiceCreate from Adobe Campaign API
layout: schema
name: ServiceCreate
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: label
  type: string
- description: ''
  name: messageType
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-service-create-schema.json
slug: adobe-campaign-standard-service-create
source_filename: adobe-campaign-standard-service-create-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-service-create-schema.json\",\n  \"title\": \"ServiceCreate\",\n  \"description\": \"ServiceCreate from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Campaign\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Campaign\"\n    },\n    \"messageType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"email\",\n        \"sms\",\n        \"push\"\n      ],\n      \"example\": \"email\"\n    }\n  },\n  \"required\": [\n    \"label\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-service-create-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: ServiceCreate
---
