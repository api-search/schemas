---
description: ''
layout: schema
name: Themes
properties_list:
- description: ''
  name: themeItems
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-themes-schema.json
slug: salesforce-themes
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"themeItems\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"colors\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"color\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"context\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"theme\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"color\",\n                \"context\",\n   \
  \             \"theme\"\n              ]\n            }\n          },\n          \"icons\": {\n            \"type\": \"array\",\n            \"description\": \"\",\n            \"example\": [],\n            \"items\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"contentType\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"height\": {\n                  \"type\": \"integer\",\n                  \"example\": 10\n                },\n                \"theme\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                },\n                \"url\": {\n                  \"type\": \"string\",\n                  \"example\": \"https://www.example.com\"\n                },\n                \"width\": {\n                  \"type\": \"integer\",\n                  \"example\": 10\n                }\n              },\n\
  \              \"required\": [\n                \"contentType\",\n                \"height\",\n                \"theme\",\n                \"url\",\n                \"width\"\n              ]\n            }\n          },\n          \"name\": {\n            \"type\": \"string\",\n            \"example\": \"Example Title\"\n          }\n        },\n        \"required\": [\n          \"colors\",\n          \"icons\",\n          \"name\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"themeItems\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Themes\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-themes-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: Themes
---
