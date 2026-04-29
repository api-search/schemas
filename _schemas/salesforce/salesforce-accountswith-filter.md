---
description: ''
layout: schema
name: AccountswithFilter
properties_list:
- description: ''
  name: data
  type: object
- description: ''
  name: errors
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-accountswith-filter-schema.json
slug: salesforce-accountswith-filter
source_filename: salesforce-accountswith-filter-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"data\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"uiapi\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"query\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"Account\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"edges\": {\n                      \"type\": \"array\",\n                      \"description\": \"\",\n                      \"example\": [],\n                      \"items\": {\n                        \"type\": \"object\"\n                      }\n                    }\n                  },\n                  \"required\": [\n                    \"edges\"\n                  ]\n                }\n              },\n              \"required\": [\n                \"Account\"\n              ]\n            }\n          },\n          \"required\": [\n    \
  \        \"query\"\n          ]\n        }\n      },\n      \"required\": [\n        \"uiapi\"\n      ]\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"data\",\n    \"errors\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"AccountswithFilter\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-accountswith-filter-schema.json
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
title: AccountswithFilter
---
