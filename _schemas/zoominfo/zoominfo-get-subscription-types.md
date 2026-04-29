---
description: ''
layout: schema
name: GetSubscriptionTypes
properties_list:
- description: ''
  name: objectTypes
  type: array
- description: ''
  name: eventTypes
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-get-subscription-types-schema.json
slug: zoominfo-get-subscription-types
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"objectTypes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"eventTypes\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"objectTypes\",\n    \"eventTypes\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GetSubscriptionTypes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-get-subscription-types-schema.json
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
title: GetSubscriptionTypes
---
