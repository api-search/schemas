---
description: ''
layout: schema
name: create
properties_list:
- description: ''
  name: sObjects
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-schema.json
slug: salesforce-create
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"sObjects\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"type\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Annual_Mileage__c\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          },\n          \"Current_Vehicle__c\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"Model_Year__c\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n        },\n        \"required\": [\n          \"type\",\n          \"Annual_Mileage__c\",\n          \"Current_Vehicle__c\",\n          \"Model_Year__c\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"sObjects\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"create\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-schema.json
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
title: create
---
