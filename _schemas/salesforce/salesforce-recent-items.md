---
description: ''
layout: schema
name: RecentItems
properties_list:
- description: ''
  name: type
  type: string
- description: ''
  name: items
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-recent-items-schema.json
slug: salesforce-recent-items
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"items\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"properties\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"id\": {\n              \"type\": \"object\",\n              \"properties\": {\n                \"type\": {\n                  \"type\": \"string\",\n                  \"example\": \"example_value\"\n                }\n              },\n              \"required\": [\n                \"type\"\n              ]\n            }\n          },\n          \"required\": [\n            \"id\"\n          ]\n        }\n      },\n      \"required\": [\n        \"type\",\n        \"properties\"\n      ]\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"items\"\n  ],\n\
  \  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecentItems\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-recent-items-schema.json
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
title: RecentItems
---
