---
description: ''
layout: schema
name: EmploymentHistory
properties_list:
- description: ''
  name: jobTitle
  type: string
- description: ''
  name: managementLevel
  type: array
- description: ''
  name: fromDate
  type: string
- description: ''
  name: toDate
  type: string
- description: ''
  name: company
  type: object
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-employment-history-schema.json
slug: zoominfo-employment-history
source_filename: zoominfo-employment-history-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobTitle\": {\n      \"type\": \"string\",\n      \"example\": \"Vice President of Sales\"\n    },\n    \"managementLevel\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"fromDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"toDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"company\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"companyId\": {\n          \"type\": \"integer\",\n          \"example\": 500123\n        },\n        \"companyName\": {\n          \"type\": \"string\",\n          \"example\": \"Acme Corporation\"\n        },\n        \"companyPhone\": {\n          \"type\": \"string\",\n          \"example\": \"+1-555-555-1234\"\n        },\n        \"companyWebsite\": {\n       \
  \   \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"companyId\",\n        \"companyName\",\n        \"companyPhone\",\n        \"companyWebsite\"\n      ]\n    }\n  },\n  \"required\": [\n    \"jobTitle\",\n    \"managementLevel\",\n    \"fromDate\",\n    \"toDate\",\n    \"company\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmploymentHistory\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-employment-history-schema.json
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
title: EmploymentHistory
---
