---
description: Standard error response
layout: schema
name: Error
properties_list:
- description: Error category
  name: category
  type: string
- description: Unique identifier for error tracking
  name: correlationId
  type: string
- description: Human-readable error message
  name: message
  type: string
- description: Specific error subcategory
  name: subCategory
  type: string
- description: Additional error context
  name: context
  type: object
- description: Links to relevant documentation
  name: links
  type: object
- description: Detailed error information
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-source-code-error-schema.json
slug: hubspot-source-code-error
source_filename: hubspot-source-code-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Standard error response\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Error category\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for error tracking\",\n      \"format\": \"uuid\",\n      \"example\": \"aeb5f871-7f07-4993-9211-075dc63e7cbf\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"Invalid input (details will vary based on the error)\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Specific error subcategory\",\n      \"example\": \"standard\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional error context\",\n      \"example\": {\n        \"missingScopes\": [\n          \"scope1\",\n       \
  \   \"scope2\"\n        ],\n        \"invalidPropertyName\": [\n          \"propertyValue\"\n        ]\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Links to relevant documentation\",\n      \"example\": {\n        \"knowledge-base\": \"https://www.hubspot.com/products/service/knowledge-base\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed error information\",\n      \"example\": [\n        {\n          \"message\": \"Required property 'path' is missing\",\n          \"code\": \"MISSING_REQUIRED_PROPERTY\",\n          \"subCategory\": \"standard\",\n          \"in\": \"body\",\n          \"context\": {\n            \"missingScopes\": [\n              \"scope1\",\n              \"scope2\"\n            ]\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed error information\",\n        \"properties\": {\n          \"message\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"Error message\",\n            \"example\": \"Required property 'path' is missing\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"Error code\",\n            \"example\": \"MISSING_REQUIRED_PROPERTY\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"Error subcategory\",\n            \"example\": \"standard\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"Location of the error\",\n            \"example\": \"body\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"description\": \"Additional context\",\n            \"example\": {\n              \"missingScopes\": [\n                \"scope1\",\n                \"scope2\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n     \
  \     \"message\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-source-code-error-schema.json
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
