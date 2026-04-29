---
description: API error response
layout: schema
name: ErrorResponse
properties_list:
- description: Machine-readable error code
  name: errorCode
  type: string
- description: Human-readable error message
  name: message
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-ui-error-response-schema.json
slug: salesforce-ui-error-response
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"API error response\",\n  \"properties\": {\n    \"errorCode\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code\",\n      \"example\": \"example_value\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorResponse\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-ui-error-response-schema.json
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
title: ErrorResponse
---
