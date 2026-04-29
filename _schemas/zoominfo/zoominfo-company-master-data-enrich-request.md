---
description: ''
layout: schema
name: CompanyMasterDataEnrichRequest
properties_list:
- description: ''
  name: matchCompanyInput
  type: array
- description: ''
  name: outputFields
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-company-master-data-enrich-request-schema.json
slug: zoominfo-company-master-data-enrich-request
source_filename: zoominfo-company-master-data-enrich-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"matchCompanyInput\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"zi_c_url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com/resource\"\n          }\n        },\n        \"required\": [\n          \"zi_c_url\"\n        ]\n      }\n    },\n    \"outputFields\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"matchCompanyInput\",\n    \"outputFields\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompanyMasterDataEnrichRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-company-master-data-enrich-request-schema.json
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
title: CompanyMasterDataEnrichRequest
---
