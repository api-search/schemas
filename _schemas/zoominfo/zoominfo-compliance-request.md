---
description: ''
layout: schema
name: ComplianceRequest
properties_list:
- description: ''
  name: matchPersonInput
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-compliance-request-schema.json
slug: zoominfo-compliance-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchPersonInput\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"companyName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"personFirstName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"personLastName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"personEmailAddress\": {\n            \"type\": \"string\",\n            \"example\": \"jsmith@example.com\"\n          }\n        }\n      }\n    }\n  },\n  \"required\": [\n    \"matchPersonInput\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ComplianceRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-compliance-request-schema.json
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
title: ComplianceRequest
---
