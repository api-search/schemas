---
description: Detailed information about a specific error
layout: schema
name: ErrorDetail
properties_list:
- description: A human-readable error message
  name: message
  type: string
- description: An error code
  name: code
  type: string
- description: A specific error subcategory
  name: subCategory
  type: string
- description: The location of the error (e.g., body, query, path)
  name: in
  type: string
- description: Additional context about the specific error
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-oauth-error-detail-schema.json
slug: hubspot-oauth-error-detail
source_filename: hubspot-oauth-error-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed information about a specific error\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message\",\n      \"example\": \"Invalid parameter value\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"An error code\",\n      \"example\": \"INVALID_PARAMETER\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"A specific error subcategory\",\n      \"example\": \"MISSING_REQUIRED_FIELD\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the error (e.g., body, query, path)\",\n      \"example\": \"body\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the specific error\",\n      \"example\": {\n        \"missingFields\": [\n          \"client_secret\"\n        ]\n      }\n    }\n  },\n \
  \ \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-oauth-error-detail-schema.json
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
