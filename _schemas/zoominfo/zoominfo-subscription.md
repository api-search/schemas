---
description: ''
layout: schema
name: Subscription
properties_list:
- description: ''
  name: eventType
  type: string
- description: ''
  name: objectType
  type: string
- description: ''
  name: fullPayload
  type: boolean
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-subscription-schema.json
slug: zoominfo-subscription
source_filename: zoominfo-subscription-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"eventType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"objectType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"fullPayload\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"eventType\",\n    \"objectType\",\n    \"fullPayload\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Subscription\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-subscription-schema.json
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
title: Subscription
---
