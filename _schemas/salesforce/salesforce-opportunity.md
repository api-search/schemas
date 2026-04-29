---
description: ''
layout: schema
name: Opportunity
properties_list:
- description: ''
  name: edges
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-opportunity-schema.json
slug: salesforce-opportunity
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"edges\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"node\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Id\": {\n                \"type\": \"string\",\n                \"example\": \"abc123\"\n              },\n              \"Name\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"value\"\n                ]\n              },\n              \"StageName\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"value\": {\n                    \"type\": \"string\",\n\
  \                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"value\"\n                ]\n              },\n              \"CloseDate\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  },\n                  \"displayValue\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"value\",\n                  \"displayValue\"\n                ]\n              },\n              \"Description\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"value\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n     \
  \             }\n                },\n                \"required\": [\n                  \"value\"\n                ]\n              }\n            },\n            \"required\": [\n              \"Id\",\n              \"Name\",\n              \"StageName\",\n              \"CloseDate\",\n              \"Description\"\n            ]\n          }\n        },\n        \"required\": [\n          \"node\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"edges\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Opportunity\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-opportunity-schema.json
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
title: Opportunity
---
