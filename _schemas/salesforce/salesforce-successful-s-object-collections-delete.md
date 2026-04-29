---
description: ''
layout: schema
name: SuccessfulSObjectCollectionsDelete
properties_list:
- description: ''
  name: id
  type: string
- description: ''
  name: success
  type: boolean
- description: ''
  name: errors
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-s-object-collections-delete-schema.json
slug: salesforce-successful-s-object-collections-delete
source_filename: salesforce-successful-s-object-collections-delete-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"id\",\n    \"success\",\n    \"errors\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulSObjectCollectionsDelete\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-s-object-collections-delete-schema.json
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
title: SuccessfulSObjectCollectionsDelete
---
