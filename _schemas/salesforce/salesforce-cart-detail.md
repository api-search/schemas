---
description: ''
layout: schema
name: CartDetail
properties_list:
- description: ''
  name: activityStartDate
  type: string
- description: ''
  name: contactId
  type: string
- description: ''
  name: transactionAmount
  type: integer
- description: ''
  name: currencyISOCode
  type: string
- description: ''
  name: cartLineDetails
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-cart-detail-schema.json
slug: salesforce-cart-detail
source_filename: salesforce-cart-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"activityStartDate\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contactId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"transactionAmount\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"currencyISOCode\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"cartLineDetails\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"cartLineProductId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"cartLineItemQuantity\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"cartLineItemAmount\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n     \
  \     \"cartLineProductCatalogId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          }\n        },\n        \"required\": [\n          \"cartLineProductId\",\n          \"cartLineItemQuantity\",\n          \"cartLineItemAmount\",\n          \"cartLineProductCatalogId\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"activityStartDate\",\n    \"contactId\",\n    \"transactionAmount\",\n    \"currencyISOCode\",\n    \"cartLineDetails\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CartDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-cart-detail-schema.json
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
title: CartDetail
---
