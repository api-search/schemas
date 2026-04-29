---
description: ''
layout: schema
name: Parentage
properties_list:
- description: ''
  name: companyId
  type: string
- description: ''
  name: companyName
  type: string
- description: ''
  name: city
  type: string
- description: ''
  name: state
  type: string
- description: ''
  name: subUnitType
  type: string
- description: ''
  name: subUnitDesc
  type: string
- description: ''
  name: acquiredByDate
  type: string
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-parentage-schema.json
slug: zoominfo-parentage
source_filename: zoominfo-parentage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"companyId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"companyName\": {\n      \"type\": \"string\",\n      \"example\": \"Acme Corporation\"\n    },\n    \"city\": {\n      \"type\": \"string\",\n      \"example\": \"San Francisco\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"example\": \"CA\"\n    },\n    \"subUnitType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"subUnitDesc\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"acquiredByDate\": {\n      \"type\": \"string\",\n      \"example\": \"2025-03-15T14:30:00Z\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Parentage\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-parentage-schema.json
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
title: Parentage
---
