---
description: ''
layout: schema
name: OrgChartEnrich
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
schema_file: json-schema/zoominfo-org-chart-enrich-schema.json
slug: zoominfo-org-chart-enrich
source_filename: zoominfo-org-chart-enrich-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"firstName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"middleName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"lastName\": {\n            \"type\": \"string\",\n            \"example\": \"Acme Corporation\"\n          },\n          \"lastUpdatedDate\"\
  : {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"example\": \"Vice President of Sales\"\n          },\n          \"hasEmail\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"hasDirectPhone\": {\n            \"type\": \"boolean\",\n            \"example\": true\n          },\n          \"department\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"jobFunction\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"orgChartTier\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"orgChartSubTier\": {\n            \"type\": \"integer\",\n            \"example\": 100\n          },\n          \"contactAccuracyScore\": {\n            \"type\": \"integer\",\n\
  \            \"example\": 85\n          },\n          \"company\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"name\"\n            ]\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"firstName\",\n          \"middleName\",\n          \"lastName\",\n          \"lastUpdatedDate\",\n          \"title\",\n          \"hasEmail\",\n          \"hasDirectPhone\",\n          \"department\",\n          \"jobFunction\",\n          \"orgChartTier\",\n          \"orgChartSubTier\",\n          \"contactAccuracyScore\",\n          \"company\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"maxResults\"\
  ,\n    \"totalResults\",\n    \"currentPage\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OrgChartEnrich\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-org-chart-enrich-schema.json
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
title: OrgChartEnrich
---
