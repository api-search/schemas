---
description: ''
layout: schema
name: UpdateWebhookRequest
properties_list:
- description: ''
  name: title
  type: string
- description: ''
  name: enabled
  type: boolean
- description: ''
  name: subscriptions
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-update-webhook-request-schema.json
slug: zoominfo-update-webhook-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"Vice President of Sales\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"subscriptionId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"objectType\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"fullPayload\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          }\n        },\n        \"required\": [\n          \"subscriptionId\",\n          \"objectType\",\n          \"fullPayload\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"title\",\n    \"enabled\",\n    \"subscriptions\"\
  \n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateWebhookRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-update-webhook-request-schema.json
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
title: UpdateWebhookRequest
---
