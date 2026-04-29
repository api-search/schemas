---
description: ''
layout: schema
name: Subscription1
properties_list:
- description: ''
  name: createdDate
  type: string
- description: ''
  name: modifiedDate
  type: string
- description: ''
  name: eventType
  type: string
- description: ''
  name: objectType
  type: string
- description: ''
  name: fullPayload
  type: boolean
- description: ''
  name: subscriptionId
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-subscription1-schema.json
slug: zoominfo-subscription1
source_filename: zoominfo-subscription1-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"createdDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"modifiedDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"eventType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"objectType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"fullPayload\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"subscriptionId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    }\n  },\n  \"required\": [\n    \"createdDate\",\n    \"modifiedDate\",\n    \"eventType\",\n    \"objectType\",\n    \"fullPayload\",\n    \"subscriptionId\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-subscription1-schema.json
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
title: Subscription1
---
