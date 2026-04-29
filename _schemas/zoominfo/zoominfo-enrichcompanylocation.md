---
description: ''
layout: schema
name: Enrichcompanylocation
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
schema_file: json-schema/zoominfo-enrichcompanylocation-schema.json
slug: zoominfo-enrichcompanylocation
source_filename: zoominfo-enrichcompanylocation-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"phone\": {\n            \"type\": \"string\",\n            \"example\": \"+1-555-555-1234\"\n          },\n          \"fax\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"street\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"city\": {\n            \"type\": \"string\",\n            \"example\": \"San Francisco\"\n          },\n          \"state\": {\n            \"\
  type\": \"string\",\n            \"example\": \"CA\"\n          },\n          \"zipCode\": {\n            \"type\": \"string\",\n            \"example\": \"94105\"\n          },\n          \"country\": {\n            \"type\": \"string\",\n            \"example\": \"US\"\n          },\n          \"company\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"addressStatus\": {\n                \"type\": \"string\",\n                \"example\": \"123 Main Street\"\n              },\n              \"subUnitType\": {\n                \"type\": \"string\",\n                \"example\": \"standard\"\n              },\n              \"locationName\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              },\n              \"locationEmployeeCount\": {\n                \"type\": \"integer\"\
  ,\n                \"example\": 250\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"addressStatus\",\n              \"subUnitType\",\n              \"locationName\",\n              \"locationEmployeeCount\"\n            ]\n          }\n        },\n        \"required\": [\n          \"phone\",\n          \"fax\",\n          \"street\",\n          \"city\",\n          \"state\",\n          \"zipCode\",\n          \"country\",\n          \"company\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"maxResults\",\n    \"totalResults\",\n    \"currentPage\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Enrichcompanylocation\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-enrichcompanylocation-schema.json
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
title: Enrichcompanylocation
---
