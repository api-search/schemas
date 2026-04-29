---
description: ''
layout: schema
name: CreateWebhookRequest
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: targetUrl
  type: string
- description: ''
  name: subscriptions
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-create-webhook-request-schema.json
slug: zoominfo-create-webhook-request
source_filename: zoominfo-create-webhook-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"Vice President of Sales\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"targetUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com/resource\"\n    },\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"eventType\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"objectType\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"fullPayload\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"eventType\",\n          \"objectType\",\n          \"fullPayload\"\
  \n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"enabled\",\n    \"targetUrl\",\n    \"subscriptions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateWebhookRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-create-webhook-request-schema.json
tags:
- B2B
- B2B Data
- Company Data
- Contact Database
- Contacts
- Data
- Lead Generation
- Marketing Intelligence
- Sales Intelligence
title: CreateWebhookRequest
---
