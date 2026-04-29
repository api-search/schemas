---
description: An error response from the Salesforce REST API, describing the problem with the request.
layout: schema
name: Error
properties_list:
- description: Human-readable description of the error.
  name: message
  type: string
- description: Salesforce error code (e.g., MALFORMED_QUERY, INVALID_FIELD, REQUIRED_FIELD_MISSING).
  name: errorCode
  type: string
- description: List of field names related to the error, if applicable (e.g., for field validation errors).
  name: fields
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-rest-error-schema.json
slug: salesforce-rest-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An error response from the Salesforce REST API, describing the problem with the request.\\n\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable description of the error.\",\n      \"example\": \"example_value\"\n    },\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Salesforce error code (e.g., MALFORMED_QUERY, INVALID_FIELD, REQUIRED_FIELD_MISSING).\\n\",\n      \"example\": \"example_value\"\n    },\n    \"fields\": {\n      \"type\": \"array\",\n      \"description\": \"List of field names related to the error, if applicable (e.g., for field validation errors).\\n\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-rest-error-schema.json
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
