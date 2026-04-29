---
description: ''
layout: schema
name: Record20
properties_list:
- description: ''
  name: referenceId
  type: string
- description: ''
  name: record
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-record20-schema.json
slug: salesforce-record20
source_filename: salesforce-record20-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"referenceId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"record\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"attributes\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"type\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            }\n          },\n          \"required\": [\n            \"type\"\n          ]\n        },\n        \"CurrencyIsoCode\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"SalesTransactionShapeId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"StartDate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"ProductId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"ProductSellingModelId\"\
  : {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"Quantity\": {\n          \"type\": \"number\",\n          \"example\": 42.5\n        },\n        \"PricingTransactionType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"EndDate\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"AdjustmentType\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"AdjustmentValue\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"AdjustmentSource\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"SalesTransactionItemShapeId\": {\n          \"type\": \"string\",\n          \"example\": \"500123\"\n        },\n        \"AdjustmentAmountScope\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n\
  \        }\n      },\n      \"required\": [\n        \"attributes\"\n      ]\n    }\n  },\n  \"required\": [\n    \"referenceId\",\n    \"record\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Record20\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-record20-schema.json
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
title: Record20
---
