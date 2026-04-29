---
description: ''
layout: schema
name: Status200-UpdateCommitmentDatabaseFailure
properties_list:
- description: ''
  name: errors
  type: array
- description: ''
  name: success
  type: boolean
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-status200-update-commitment-database-failure-schema.json
slug: salesforce-status200-update-commitment-database-failure
source_filename: salesforce-status200-update-commitment-database-failure-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    },\n    \"success\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    }\n  },\n  \"required\": [\n    \"errors\",\n    \"success\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Status200-UpdateCommitmentDatabaseFailure\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-status200-update-commitment-database-failure-schema.json
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
title: Status200-UpdateCommitmentDatabaseFailure
---
