---
description: ''
layout: schema
name: EligiblePromotionsRequest
properties_list:
- description: ''
  name: cart
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-eligible-promotions-request-schema.json
slug: salesforce-eligible-promotions-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"cart\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"cartDetails\": {\n          \"type\": \"array\",\n          \"description\": \"\",\n          \"example\": [],\n          \"items\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"activityStartDate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"contactId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"transactionAmount\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              },\n              \"currencyISOCode\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"cartLineDetails\": {\n                \"type\": \"array\",\n                \"description\"\
  : \"\",\n                \"example\": [],\n                \"items\": {\n                  \"type\": \"object\",\n                  \"properties\": {\n                    \"cartLineProductId\": {\n                      \"type\": \"object\"\n                    },\n                    \"cartLineItemQuantity\": {\n                      \"type\": \"object\"\n                    },\n                    \"cartLineItemAmount\": {\n                      \"type\": \"object\"\n                    },\n                    \"cartLineProductCatalogId\": {\n                      \"type\": \"object\"\n                    }\n                  },\n                  \"required\": [\n                    \"cartLineProductId\",\n                    \"cartLineItemQuantity\",\n                    \"cartLineItemAmount\",\n                    \"cartLineProductCatalogId\"\n                  ]\n                }\n              }\n            },\n            \"required\": [\n              \"activityStartDate\",\n\
  \              \"contactId\",\n              \"transactionAmount\",\n              \"currencyISOCode\",\n              \"cartLineDetails\"\n            ]\n          }\n        }\n      },\n      \"required\": [\n        \"cartDetails\"\n      ]\n    }\n  },\n  \"required\": [\n    \"cart\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EligiblePromotionsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-eligible-promotions-request-schema.json
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
title: EligiblePromotionsRequest
---
