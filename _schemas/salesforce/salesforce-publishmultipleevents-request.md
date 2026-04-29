---
description: ''
layout: schema
name: PublishmultipleeventsRequest
properties_list:
- description: ''
  name: allOrNone
  type: boolean
- description: ''
  name: compositeRequest
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-publishmultipleevents-request-schema.json
slug: salesforce-publishmultipleevents-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"allOrNone\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"compositeRequest\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"method\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          },\n          \"referenceId\": {\n            \"type\": \"string\",\n            \"example\": \"500123\"\n          },\n          \"body\": {\n            \"type\": \"object\",\n            \"properties\": {\n              \"Annual_Mileage__c\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              },\n              \"Current_Vehicle__c\": {\n                \"type\": \"string\",\n     \
  \           \"example\": \"example_value\"\n              },\n              \"Model_Year__c\": {\n                \"type\": \"integer\",\n                \"example\": 10\n              }\n            },\n            \"required\": [\n              \"Annual_Mileage__c\",\n              \"Current_Vehicle__c\",\n              \"Model_Year__c\"\n            ]\n          }\n        },\n        \"required\": [\n          \"method\",\n          \"url\",\n          \"referenceId\",\n          \"body\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"allOrNone\",\n    \"compositeRequest\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishmultipleeventsRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-publishmultipleevents-request-schema.json
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
title: PublishmultipleeventsRequest
---
