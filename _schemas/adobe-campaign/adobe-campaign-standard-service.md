---
description: Service from Adobe Campaign API
layout: schema
name: Service
properties_list:
- description: Unique identifier for the service.
  name: PKey
  type: string
- description: Internal name of the service.
  name: name
  type: string
- description: Display label of the service.
  name: label
  type: string
- description: Default channel for the service.
  name: messageType
  type: string
- description: Service start date.
  name: start
  type: string
- description: Service end date.
  name: end
  type: string
- description: ''
  name: created
  type: string
- description: ''
  name: lastModified
  type: string
provider_name: Adobe Campaign
provider_slug: adobe-campaign
schema_file: json-schema/adobe-campaign-standard-service-schema.json
slug: adobe-campaign-standard-service
source_filename: adobe-campaign-standard-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-service-schema.json\",\n  \"title\": \"Service\",\n  \"description\": \"Service from Adobe Campaign API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"PKey\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the service.\",\n      \"readOnly\": true,\n      \"example\": \"example_value\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Internal name of the service.\",\n      \"example\": \"Example Campaign\"\n    },\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label of the service.\",\n      \"example\": \"Example Campaign\"\n    },\n    \"messageType\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"email\",\n        \"sms\",\n        \"push\"\n      ],\n     \
  \ \"description\": \"Default channel for the service.\",\n      \"example\": \"email\"\n    },\n    \"start\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Service start date.\",\n      \"example\": \"example_value\"\n    },\n    \"end\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"description\": \"Service end date.\",\n      \"example\": \"example_value\"\n    },\n    \"created\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"example\": \"example_value\"\n    },\n    \"lastModified\": {\n      \"type\": \"string\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"example\": \"example_value\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/adobe-campaign/refs/heads/main/json-schema/adobe-campaign-standard-service-schema.json
tags:
- Campaign Management
- Customer Experience
- Email Marketing
- Marketing Automation
- Multi-Channel Marketing
title: Service
---
