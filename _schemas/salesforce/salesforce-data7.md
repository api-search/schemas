---
description: ''
layout: schema
name: Data7
properties_list:
- description: ''
  name: uiapi
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-data7-schema.json
slug: salesforce-data7
source_filename: salesforce-data7-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"uiapi\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"query\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"Opportunity\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"edges\": {\n                  \"type\": \"array\",\n                  \"description\": \"\",\n                  \"example\": [],\n                  \"items\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"node\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"node\"\n                    ]\n                  }\n                }\n              },\n              \"required\": [\n                \"edges\"\n              ]\n            }\n          },\n          \"required\": [\n       \
  \     \"Opportunity\"\n          ]\n        }\n      },\n      \"required\": [\n        \"query\"\n      ]\n    }\n  },\n  \"required\": [\n    \"uiapi\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Data7\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-data7-schema.json
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
title: Data7
---
