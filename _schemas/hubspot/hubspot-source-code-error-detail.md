---
description: Detailed error information
layout: schema
name: ErrorDetail
properties_list:
- description: Error message
  name: message
  type: string
- description: Error code
  name: code
  type: string
- description: Error subcategory
  name: subCategory
  type: string
- description: Location of the error
  name: in
  type: string
- description: Additional context
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-source-code-error-detail-schema.json
slug: hubspot-source-code-error-detail
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed error information\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"Required property 'path' is missing\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code\",\n      \"example\": \"MISSING_REQUIRED_PROPERTY\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Error subcategory\",\n      \"example\": \"standard\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"Location of the error\",\n      \"example\": \"body\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context\",\n      \"example\": {\n        \"missingScopes\": [\n          \"scope1\",\n          \"scope2\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\"\
  ,\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-source-code-error-detail-schema.json
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
