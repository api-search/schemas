---
description: ''
layout: schema
name: DecisionTable
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: parameters
  type: array
- description: ''
  name: sourceCriteria
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-decision-table-schema.json
slug: salesforce-decision-table
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"sourceCriteria\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"parameters\",\n    \"sourceCriteria\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DecisionTable\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-decision-table-schema.json
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
title: DecisionTable
---
