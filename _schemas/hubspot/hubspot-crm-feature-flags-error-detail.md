---
description: Detailed error information for specific validation failures
layout: schema
name: ErrorDetail
properties_list:
- description: Specific error message
  name: message
  type: string
- description: Error code
  name: code
  type: string
- description: Error sub-category
  name: subCategory
  type: string
- description: Location of the error (e.g., path, body, query)
  name: in
  type: string
- description: Additional context for the error
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-error-detail-schema.json
slug: hubspot-crm-feature-flags-error-detail
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed error information for specific validation failures\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Specific error message\",\n      \"example\": \"flagState is required\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code\",\n      \"example\": \"REQUIRED_FIELD\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Error sub-category\",\n      \"example\": \"MISSING_FIELD\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"Location of the error (e.g., path, body, query)\",\n      \"example\": \"body\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context for the error\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-error-detail-schema.json
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
