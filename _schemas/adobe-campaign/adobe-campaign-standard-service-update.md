---
description: ServiceUpdate from Adobe Campaign API
layout: schema
name: ServiceUpdate
properties_list:
- description: ''
  name: label
  type: string
- description: ''
  name: messageType
  type: string
- description: ''
  name: start
  type: string
- description: ''
  name: end
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-service-update-schema.json
slug: adobe-campaign-standard-service-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-service-update-schema.json\",\n  \"title\": \"ServiceUpdate\",\n  \"description\": \"ServiceUpdate from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"example\": \"Example Campaign\"\n    },\n    \"messageType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"email\",\n        \"sms\",\n        \"push\"\n      ],\n      \"example\": \"email\"\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"example_value\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-service-update-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: ServiceUpdate
---
