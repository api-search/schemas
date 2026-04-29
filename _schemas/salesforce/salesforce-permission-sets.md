---
description: ''
layout: schema
name: PermissionSets
properties_list:
- description: ''
  name: Max
  type: integer
- description: ''
  name: Remaining
  type: integer
- description: ''
  name: CreateCustom
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-permission-sets-schema.json
slug: salesforce-permission-sets
source_filename: salesforce-permission-sets-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"Max\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"Remaining\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"CreateCustom\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"Max\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        },\n        \"Remaining\": {\n          \"type\": \"integer\",\n          \"example\": 10\n        }\n      },\n      \"required\": [\n        \"Max\",\n        \"Remaining\"\n      ]\n    }\n  },\n  \"required\": [\n    \"Max\",\n    \"Remaining\",\n    \"CreateCustom\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PermissionSets\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-permission-sets-schema.json
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
title: PermissionSets
---
