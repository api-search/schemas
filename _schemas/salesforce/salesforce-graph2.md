---
description: ''
layout: schema
name: Graph2
properties_list:
- description: ''
  name: graphId
  type: string
- description: ''
  name: records
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-graph2-schema.json
slug: salesforce-graph2
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"graphId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"records\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"referenceId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"record\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"attributes\": {\n                \"type\": \"object\",\n                \"properties\": {\n                  \"type\": {\n                    \"type\": \"string\",\n                    \"example\": \"example_value\"\n                  }\n                },\n                \"required\": [\n                  \"type\"\n                ]\n              },\n              \"CurrencyIsoCode\": {\n                \"type\": \"string\",\n              \
  \  \"example\": \"example_value\"\n              },\n              \"SalesTransactionShapeId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"StartDate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"ProductId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"ProductSellingModelId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"Quantity\": {\n                \"type\": \"number\",\n                \"example\": 42.5\n              },\n              \"PricingTransactionType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"EndDate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n   \
  \           }\n            },\n            \"required\": [\n              \"attributes\",\n              \"CurrencyIsoCode\"\n            ]\n          }\n        },\n        \"required\": [\n          \"referenceId\",\n          \"record\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"graphId\",\n    \"records\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Graph2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-graph2-schema.json
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
title: Graph2
---
