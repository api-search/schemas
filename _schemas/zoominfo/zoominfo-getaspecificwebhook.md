---
description: ''
layout: schema
name: Getaspecificwebhook
properties_list:
- description: ''
  name: id
  type: string
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
  name: createdDate
  type: string
- description: ''
  name: subscriptions
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-getaspecificwebhook-schema.json
slug: zoominfo-getaspecificwebhook
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"title\": {\n      \"type\": \"string\",\n      \"example\": \"Vice President of Sales\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"targetUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com/resource\"\n    },\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"subscriptions\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"createdDate\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"modifiedDate\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n\
  \          \"eventType\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"objectType\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"fullPayload\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"subscriptionId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"createdDate\",\n          \"modifiedDate\",\n          \"eventType\",\n          \"objectType\",\n          \"fullPayload\",\n          \"subscriptionId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"title\",\n    \"enabled\",\n    \"targetUrl\",\n    \"createdDate\",\n    \"subscriptions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Getaspecificwebhook\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-getaspecificwebhook-schema.json
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
title: Getaspecificwebhook
---
