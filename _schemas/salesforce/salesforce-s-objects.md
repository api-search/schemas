---
description: ''
layout: schema
name: sObjects
properties_list:
- description: ''
  name: type
  type: string
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
schema_file: json-schema/salesforce-s-objects-schema.json
slug: salesforce-s-objects
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Annual_Mileage__c\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"Current_Vehicle__c\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"Model_Year__c\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"type\",\n    \"Annual_Mileage__c\",\n    \"Current_Vehicle__c\",\n    \"Model_Year__c\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"sObjects\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-s-objects-schema.json
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
title: sObjects
---
