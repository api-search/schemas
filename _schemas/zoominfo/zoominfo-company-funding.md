---
description: ''
layout: schema
name: CompanyFunding
properties_list:
- description: ''
  name: date
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: amount
  type: integer
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-company-funding-schema.json
slug: zoominfo-company-funding
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"date\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"amount\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    }\n  },\n  \"required\": [\n    \"date\",\n    \"type\",\n    \"amount\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompanyFunding\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-company-funding-schema.json
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
title: CompanyFunding
---
