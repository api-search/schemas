---
description: ''
layout: schema
name: PublishsingleeventRequest
properties_list:
- description: ''
  name: Annual_Mileage__c
  type: integer
- description: ''
  name: Current_Vehicle__c
  type: string
- description: ''
  name: Model_Year__c
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-publishsingleevent-request-schema.json
slug: salesforce-publishsingleevent-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Annual_Mileage__c\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"Current_Vehicle__c\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Model_Year__c\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"Annual_Mileage__c\",\n    \"Current_Vehicle__c\",\n    \"Model_Year__c\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PublishsingleeventRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-publishsingleevent-request-schema.json
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
title: PublishsingleeventRequest
---
