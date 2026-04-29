---
description: ''
layout: schema
name: EmployeeGrowth1
properties_list:
- description: ''
  name: oneYearGrowthRate
  type: string
- description: ''
  name: twoYearGrowthRate
  type: string
- description: ''
  name: employeeGrowthDataPoints
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-employee-growth1-schema.json
slug: zoominfo-employee-growth1
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"oneYearGrowthRate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"twoYearGrowthRate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"employeeGrowthDataPoints\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\"\n      }\n    }\n  },\n  \"required\": [\n    \"oneYearGrowthRate\",\n    \"twoYearGrowthRate\",\n    \"employeeGrowthDataPoints\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EmployeeGrowth1\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-employee-growth1-schema.json
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
title: EmployeeGrowth1
---
