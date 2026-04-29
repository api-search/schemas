---
description: ''
layout: schema
name: Detail4
properties_list:
- description: ''
  name: success
  type: boolean
- description: ''
  name: errors
  type: object
- description: ''
  name: links
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-detail4-schema.json
slug: salesforce-detail4
source_filename: salesforce-detail4-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"errors\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"field\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"message\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        }\n      },\n      \"required\": [\n        \"field\",\n        \"message\"\n      ]\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"gifttransaction\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"href\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"id\": {\n              \"type\": \"string\",\n              \"example\": \"abc123\"\n            }\n          },\n          \"required\": [\n            \"href\",\n    \
  \        \"id\"\n          ]\n        }\n      },\n      \"required\": [\n        \"gifttransaction\"\n      ]\n    }\n  },\n  \"required\": [\n    \"success\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Detail4\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-detail4-schema.json
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
title: Detail4
---
