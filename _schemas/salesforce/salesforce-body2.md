---
description: ''
layout: schema
name: Body2
properties_list:
- description: ''
  name: Name
  type: string
- description: ''
  name: Custom__c
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-body2-schema.json
slug: salesforce-body2
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"example\": \"Example Title\"\n    },\n    \"Custom__c\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"Name\",\n    \"Custom__c\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Body2\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-body2-schema.json
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
title: Body2
---
