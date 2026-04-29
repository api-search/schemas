---
description: ''
layout: schema
name: CompositeRequest3
properties_list:
- description: ''
  name: method
  type: string
- description: ''
  name: url
  type: string
- description: ''
  name: referenceId
  type: string
- description: ''
  name: body
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-composite-request3-schema.json
slug: salesforce-composite-request3
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"method\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"referenceId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"body\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Annual_Mileage__c\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Current_Vehicle__c\": {\n          \"type\": \"string\",\n          \"example\": \"example_value\"\n        },\n        \"Model_Year__c\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Annual_Mileage__c\",\n        \"Current_Vehicle__c\",\n        \"Model_Year__c\"\n      ]\n    }\n  },\n  \"required\": [\n    \"method\",\n    \"url\",\n    \"referenceId\",\n    \"body\"\n  ],\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CompositeRequest3\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-composite-request3-schema.json
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
title: CompositeRequest3
---
