---
description: Standard error response object
layout: schema
name: Error
properties_list:
- description: The category of the error
  name: category
  type: string
- description: A unique identifier for tracking this error
  name: correlationId
  type: string
- description: A human-readable error message
  name: message
  type: string
- description: A more specific error category
  name: subCategory
  type: string
- description: Additional context about the error
  name: context
  type: object
- description: Links to relevant documentation
  name: links
  type: object
- description: List of specific errors
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-oauth-error-schema.json
slug: hubspot-oauth-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Standard error response object\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The category of the error\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for tracking this error\",\n      \"format\": \"uuid\",\n      \"example\": \"aeb5f871-7f07-4993-9211-075dc63e7cbf\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message\",\n      \"example\": \"Invalid refresh token\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"A more specific error category\",\n      \"example\": \"INVALID_TOKEN\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the error\",\n      \"example\": {\n        \"invalidToken\": [\n          \"The provided\
  \ token is invalid or expired\"\n        ]\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Links to relevant documentation\",\n      \"example\": {\n        \"knowledge-base\": \"https://developers.hubspot.com/docs/api/oauth\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of specific errors\",\n      \"example\": [\n        {\n          \"message\": \"Invalid parameter value\",\n          \"code\": \"INVALID_PARAMETER\",\n          \"subCategory\": \"MISSING_REQUIRED_FIELD\",\n          \"in\": \"body\",\n          \"context\": {\n            \"missingFields\": [\n              \"client_secret\"\n            ]\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed information about a specific error\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"A human-readable\
  \ error message\",\n            \"example\": \"Invalid parameter value\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"An error code\",\n            \"example\": \"INVALID_PARAMETER\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"A specific error subcategory\",\n            \"example\": \"MISSING_REQUIRED_FIELD\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"The location of the error (e.g., body, query, path)\",\n            \"example\": \"body\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"description\": \"Additional context about the specific error\",\n            \"example\": {\n              \"missingFields\": [\n                \"client_secret\"\n              ]\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n\
  \      }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-oauth-error-schema.json
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
