---
description: Detailed information about a specific error.
layout: schema
name: ErrorDetail
properties_list:
- description: Human-readable error message
  name: message
  type: string
- description: Error code
  name: code
  type: string
- description: Error subcategory
  name: subCategory
  type: string
- description: Location where error occurred
  name: in
  type: string
- description: ''
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-error-detail-schema.json
slug: hubspot-conversations-error-detail
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed information about a specific error.\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"Invalid thread ID format\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code\",\n      \"example\": \"INVALID_FORMAT\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Error subcategory\",\n      \"example\": \"PARAMETER_ERROR\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"Location where error occurred\",\n      \"example\": \"path\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-error-detail-schema.json
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
