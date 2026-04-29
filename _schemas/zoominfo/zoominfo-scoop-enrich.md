---
description: ''
layout: schema
name: ScoopEnrich
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
schema_file: json-schema/zoominfo-scoop-enrich-schema.json
slug: zoominfo-scoop-enrich
source_filename: zoominfo-scoop-enrich-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"totalResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"id\": {\n            \"type\": \"integer\",\n            \"example\": 500123\n          },\n          \"publishedDate\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"originalPublishedDate\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"linkText\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n         \
  \ \"link\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"description\": {\n            \"type\": \"string\",\n            \"example\": \"Enterprise software company\"\n          },\n          \"topics\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"updateText\": {\n            \"type\": \"string\",\n            \"example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"types\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                },\n                \"type\": {\n                  \"type\": \"string\"\
  ,\n                  \"example\": \"standard\"\n                }\n              },\n              \"required\": [\n                \"id\",\n                \"type\"\n              ]\n            }\n          },\n          \"contacts\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"company\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"integer\",\n                \"example\": 500123\n              },\n              \"name\": {\n                \"type\": \"string\",\n                \"example\": \"Acme Corporation\"\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"name\"\n            ]\n          }\n        },\n        \"required\": [\n          \"id\",\n          \"publishedDate\",\n          \"originalPublishedDate\"\
  ,\n          \"linkText\",\n          \"link\",\n          \"description\",\n          \"topics\",\n          \"updateText\",\n          \"types\",\n          \"contacts\",\n          \"company\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"maxResults\",\n    \"totalResults\",\n    \"currentPage\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ScoopEnrich\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-scoop-enrich-schema.json
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
title: ScoopEnrich
---
