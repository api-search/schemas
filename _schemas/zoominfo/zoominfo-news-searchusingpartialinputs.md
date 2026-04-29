---
description: ''
layout: schema
name: NewsSearchusingpartialinputs
properties_list:
- description: ''
  name: currentPage
  type: integer
- description: ''
  name: maxResults
  type: integer
- description: ''
  name: data
  type: array
provider_name: ZoomInfo
provider_slug: zoominfo
schema_file: json-schema/zoominfo-news-searchusingpartialinputs-schema.json
slug: zoominfo-news-searchusingpartialinputs
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentPage\": {\n      \"type\": \"integer\",\n      \"example\": 1\n    },\n    \"maxResults\": {\n      \"type\": \"integer\",\n      \"example\": 100\n    },\n    \"data\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"domain\": {\n            \"type\": \"string\",\n            \"example\": \"example.com\"\n          },\n          \"title\": {\n            \"type\": \"string\",\n            \"example\": \"Vice President of Sales\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com/resource\"\n          },\n          \"imageUrl\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com/resource\"\n          },\n          \"pageDate\": {\n            \"type\": \"string\",\n            \"\
  example\": \"2025-03-15T14:30:00Z\"\n          },\n          \"categories\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"string\"\n            }\n          },\n          \"company\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"id\": {\n                  \"type\": \"integer\",\n                  \"example\": 500123\n                },\n                \"name\": {\n                  \"type\": \"string\",\n                  \"example\": \"Acme Corporation\"\n                }\n              },\n              \"required\": [\n                \"id\",\n                \"name\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"domain\",\n          \"title\",\n         \
  \ \"url\",\n          \"pageDate\",\n          \"categories\",\n          \"company\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"currentPage\",\n    \"maxResults\",\n    \"data\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NewsSearchusingpartialinputs\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/zoominfo/refs/heads/main/json-schema/zoominfo-news-searchusingpartialinputs-schema.json
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
title: NewsSearchusingpartialinputs
---
