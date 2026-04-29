---
description: ''
layout: schema
name: CreateOrderEvergreenTermedRequest
properties_list:
- description: ''
  name: allOrNone
  type: boolean
- description: ''
  name: compositeRequest
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-order-evergreen-termed-request-schema.json
slug: salesforce-create-order-evergreen-termed-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"allOrNone\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"compositeRequest\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"method\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"referenceId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"body\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"AccountId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"EffectiveDate\": {\n                \"type\": \"string\",\n           \
  \     \"example\": \"example_value\"\n              },\n              \"Pricebook2Id\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"BillToContactId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"Status\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"AppUsageType\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"RecordId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"OrderId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"Type\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n           \
  \   \"OrderActionId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"PricebookEntryId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"Quantity\": {\n                \"type\": \"number\",\n                \"example\": 42.5\n              },\n              \"UnitPrice\": {\n                \"type\": \"number\",\n                \"example\": 42.5\n              },\n              \"NetUnitPrice\": {\n                \"type\": \"number\",\n                \"example\": 42.5\n              },\n              \"TotalLineAmount\": {\n                \"type\": \"number\",\n                \"example\": 42\n              },\n              \"PeriodBoundary\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"BillingFrequency2\": {\n                \"type\": \"string\",\n               \
  \ \"example\": \"example_value\"\n              },\n              \"ServiceDate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              },\n              \"TaxTreatmentId\": {\n                \"type\": \"string\",\n                \"example\": \"500123\"\n              },\n              \"PricingTermCount\": {\n                \"type\": \"number\",\n                \"example\": 42\n              },\n              \"EndDate\": {\n                \"type\": \"string\",\n                \"example\": \"example_value\"\n              }\n            }\n          }\n        },\n        \"required\": [\n          \"method\",\n          \"url\",\n          \"referenceId\",\n          \"body\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"allOrNone\",\n    \"compositeRequest\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateOrderEvergreenTermedRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-order-evergreen-termed-request-schema.json
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
title: CreateOrderEvergreenTermedRequest
---
