---
description: ''
layout: schema
name: BulkCompanySearchRequest
properties_list:
- description: ''
  name: jobType
  type: string
- description: ''
  name: query
  type: object
- description: ''
  name: outputFields
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-bulk-company-search-request-schema.json
slug: zoominfo-bulk-company-search-request
source_filename: zoominfo-bulk-company-search-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"jobType\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"query\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"address\": {\n          \"type\": \"string\",\n          \"example\": \"123 Main Street\"\n        }\n      },\n      \"required\": [\n        \"address\"\n      ]\n    },\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"jobType\",\n    \"query\",\n    \"outputFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BulkCompanySearchRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-bulk-company-search-request-schema.json
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
title: BulkCompanySearchRequest
---
