---
description: ''
layout: schema
name: Query
properties_list:
- description: ''
  name: Account
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-query-schema.json
slug: salesforce-query
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Account\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"edges\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"node\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"Id\": {\n                    \"type\": \"string\",\n                    \"example\": \"abc123\"\n                  },\n                  \"Name\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"value\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"value\"\n                    ]\n                  }\n                },\n                \"required\": [\n       \
  \           \"Id\",\n                  \"Name\"\n                ]\n              }\n            },\n            \"required\": [\n              \"node\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"edges\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Account\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Query\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-query-schema.json
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
title: Query
---
