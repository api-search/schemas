---
description: An error response from the Salesforce Bulk API 2.0.
layout: schema
name: Error
properties_list:
- description: Human-readable description of the error.
  name: message
  type: string
- description: Salesforce error code identifying the type of error.
  name: errorCode
  type: string
- description: List of field names related to the error, if applicable.
  name: fields
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-bulk-2-error-schema.json
slug: salesforce-bulk-2-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An error response from the Salesforce Bulk API 2.0.\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the error.\",\n      \"example\": \"example_value\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce error code identifying the type of error.\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"List of field names related to the error, if applicable.\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-bulk-2-error-schema.json
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
title: Error
---
