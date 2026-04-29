---
description: ''
layout: schema
name: Uiapi7
properties_list:
- description: ''
  name: query
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-uiapi7-schema.json
slug: salesforce-uiapi7
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"query\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Opportunity\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"edges\": {\n              \"type\": \"array\",\n              \"description\": \"\",\n              \"example\": [],\n              \"items\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"node\": {\n                    \"type\": \"object\",\n                    \"properties\": {\n                      \"Id\": {\n                        \"type\": \"object\"\n                      },\n                      \"Name\": {\n                        \"type\": \"object\"\n                      },\n                      \"StageName\": {\n                        \"type\": \"object\"\n                      },\n                      \"CloseDate\": {\n                        \"type\": \"object\"\n                   \
  \   },\n                      \"Description\": {\n                        \"type\": \"object\"\n                      }\n                    },\n                    \"required\": [\n                      \"Id\",\n                      \"Name\",\n                      \"StageName\",\n                      \"CloseDate\",\n                      \"Description\"\n                    ]\n                  }\n                },\n                \"required\": [\n                  \"node\"\n                ]\n              }\n            }\n          },\n          \"required\": [\n            \"edges\"\n          ]\n        }\n      },\n      \"required\": [\n        \"Opportunity\"\n      ]\n    }\n  },\n  \"required\": [\n    \"query\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Uiapi7\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-uiapi7-schema.json
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
title: Uiapi7
---
