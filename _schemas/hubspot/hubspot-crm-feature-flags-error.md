---
description: Represents an error response from the API
layout: schema
name: Error
properties_list:
- description: The error category
  name: category
  type: string
- description: Unique identifier for the request, useful for debugging
  name: correlationId
  type: string
- description: Human-readable error message
  name: message
  type: string
- description: More specific error classification
  name: subCategory
  type: string
- description: Additional context about the error
  name: context
  type: object
- description: Helpful links related to the error
  name: links
  type: object
- description: List of detailed error information
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-feature-flags-error-schema.json
slug: hubspot-crm-feature-flags-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents an error response from the API\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The error category\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for the request, useful for debugging\",\n      \"format\": \"uuid\",\n      \"example\": \"aeb5f871-7f07-4993-9211-075dc63e7cbf\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"Invalid input JSON\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"More specific error classification\",\n      \"example\": \"INVALID_PARAMETER\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the error\",\n      \"example\": {\n        \"key\": \"value\"\n\
  \      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Helpful links related to the error\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of detailed error information\",\n      \"example\": [\n        {\n          \"message\": \"flagState is required\",\n          \"code\": \"REQUIRED_FIELD\",\n          \"subCategory\": \"MISSING_FIELD\",\n          \"in\": \"body\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed error information for specific validation failures\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Specific error message\",\n            \"example\": \"flagState is required\"\n          },\n          \"code\": {\n            \"type\": \"\
  string\",\n            \"description\": \"Error code\",\n            \"example\": \"REQUIRED_FIELD\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"Error sub-category\",\n            \"example\": \"MISSING_FIELD\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"Location of the error (e.g., path, body, query)\",\n            \"example\": \"body\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"description\": \"Additional context for the error\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-feature-flags-error-schema.json
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
