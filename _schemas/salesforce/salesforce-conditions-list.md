---
description: ''
layout: schema
name: ConditionsList
properties_list:
- description: ''
  name: fieldName
  type: string
- description: ''
  name: value
  type: object
- description: ''
  name: operator
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-conditions-list-schema.json
slug: salesforce-conditions-list
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"fieldName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"value\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"operator\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"fieldName\",\n    \"value\",\n    \"operator\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ConditionsList\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-conditions-list-schema.json
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
title: ConditionsList
---
