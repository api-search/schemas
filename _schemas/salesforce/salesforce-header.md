---
description: ''
layout: schema
name: Header
properties_list:
- description: ''
  name: isRichText
  type: '[''string'', ''null'']'
- description: ''
  name: messageSegments
  type: array
- description: ''
  name: text
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-header-schema.json
slug: salesforce-header
source_filename: salesforce-header-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"isRichText\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"example_value\"\n    },\n    \"messageSegments\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"motif\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"color\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"largeIconUrl\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              },\n              \"mediumIconUrl\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              },\n              \"smallIconUrl\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\
  \n              },\n              \"svgIconUrl\": {\n                \"type\": \"['string', 'null']\",\n                \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"color\",\n              \"largeIconUrl\",\n              \"mediumIconUrl\",\n              \"smallIconUrl\",\n              \"svgIconUrl\"\n            ]\n          },\n          \"reference\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"url\": {\n                \"type\": \"string\",\n                \"example\": \"https://www.example.com\"\n              }\n            },\n            \"required\": [\n              \"id\",\n              \"url\"\n            ]\n          },\n          \"text\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n\
  \          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"motif\",\n          \"reference\",\n          \"text\",\n          \"type\"\n        ]\n      }\n    },\n    \"text\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"isRichText\",\n    \"messageSegments\",\n    \"text\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Header\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-header-schema.json
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
title: Header
---
