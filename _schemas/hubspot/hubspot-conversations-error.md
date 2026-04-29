---
description: Standard error response structure.
layout: schema
name: Error
properties_list:
- description: Error category
  name: category
  type: string
- description: Unique tracking identifier for support requests
  name: correlationId
  type: string
- description: Human-readable error message
  name: message
  type: string
- description: Error subcategory
  name: subCategory
  type: string
- description: ''
  name: context
  type: object
- description: ''
  name: links
  type: object
- description: ''
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-conversations-error-schema.json
slug: hubspot-conversations-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Standard error response structure.\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Error category\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique tracking identifier for support requests\",\n      \"format\": \"uuid\",\n      \"example\": \"aeb5f871-7f07-4993-9211-075dc63e7cbf\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"Invalid input parameters\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Error subcategory\",\n      \"example\": \"INVALID_PARAMETER\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"example\": {\n      \
  \  \"key\": \"value\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"message\": \"Invalid thread ID format\",\n          \"code\": \"INVALID_FORMAT\",\n          \"subCategory\": \"PARAMETER_ERROR\",\n          \"in\": \"path\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed information about a specific error.\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable error message\",\n            \"example\": \"Invalid thread ID format\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"Error code\",\n            \"example\": \"INVALID_FORMAT\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"Error subcategory\"\
  ,\n            \"example\": \"PARAMETER_ERROR\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"Location where error occurred\",\n            \"example\": \"path\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-conversations-error-schema.json
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
title: Error
---
