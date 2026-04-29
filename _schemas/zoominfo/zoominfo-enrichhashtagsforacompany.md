---
description: ''
layout: schema
name: Enrichhashtagsforacompany
properties_list:
- description: ''
  name: maxResults
  type: integer
- description: ''
  name: totalResults
  type: integer
- description: ''
  name: currentPage
  type: integer
- description: ''
  name: data
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-enrichhashtagsforacompany-schema.json
slug: zoominfo-enrichhashtagsforacompany
source_filename: zoominfo-enrichhashtagsforacompany-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"tag\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"external_id\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"500123\"\n          },\n          \"searchString\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          },\n \
  \         \"group\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"score\": {\n            \"type\": \"['string', 'null']\",\n            \"example\": \"example_value\"\n          },\n          \"priority\": {\n            \"type\": \"object\",\n            \"example\": \"example_value\"\n          },\n          \"parentCategory\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"categorizedFlag\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"label\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"tag\",\n          \"external_id\",\n          \"searchString\",\n          \"description\",\n          \"group\",\n          \"score\",\n          \"priority\",\n          \"parentCategory\",\n          \"categorizedFlag\",\n  \
  \        \"label\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"maxResults\",\n    \"totalResults\",\n    \"currentPage\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enrichhashtagsforacompany\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-enrichhashtagsforacompany-schema.json
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
title: Enrichhashtagsforacompany
---
