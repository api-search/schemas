---
description: Detailed information about a specific error
layout: schema
name: ErrorDetail
properties_list:
- description: Human-readable error message
  name: message
  type: string
- description: Machine-readable error code
  name: code
  type: string
- description: Specific error subcategory
  name: subCategory
  type: string
- description: Location where the error occurred (e.g., query, path, body)
  name: in
  type: string
- description: Additional context about the specific error
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-analytics-events-error-detail-schema.json
slug: hubspot-analytics-events-error-detail
source_filename: hubspot-analytics-events-error-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed information about a specific error\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"This is an example description.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Machine-readable error code\",\n      \"example\": \"example-value\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Specific error subcategory\",\n      \"example\": \"standard\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"Location where the error occurred (e.g., query, path, body)\",\n      \"example\": \"example-value\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the specific error\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"message\"\
  \n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-analytics-events-error-detail-schema.json
tags:
- Analytics
- Commerce
- Content
- CRM
- Customer Service
- Email Marketing
- Marketing
- Marketing Automation
- Operations
- Sales
title: ErrorDetail
---
