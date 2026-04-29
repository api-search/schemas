---
description: Standard error response returned when an API request fails
layout: schema
name: Error
properties_list:
- description: High-level error category
  name: category
  type: string
- description: Unique identifier for tracking and debugging the error
  name: correlationId
  type: string
- description: Human-readable error message
  name: message
  type: string
- description: Specific error subcategory for detailed classification
  name: subCategory
  type: string
- description: Additional context about the error
  name: context
  type: object
- description: Relevant links for error resolution and documentation
  name: links
  type: object
- description: List of specific errors encountered
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-analytics-events-error-schema.json
slug: hubspot-analytics-events-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Standard error response returned when an API request fails\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"High-level error category\",\n      \"example\": \"standard\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier for tracking and debugging the error\",\n      \"format\": \"uuid\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"This is an example description.\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Specific error subcategory for detailed classification\",\n      \"example\": \"standard\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the error\",\n      \"example\"\
  : {\n        \"key\": \"value\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Relevant links for error resolution and documentation\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"List of specific errors encountered\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"code\": \"example-value\",\n          \"subCategory\": \"standard\",\n          \"in\": \"example-value\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed information about a specific error\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Human-readable error message\",\n            \"example\": \"This is an example description.\"\
  \n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"Machine-readable error code\",\n            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"Specific error subcategory\",\n            \"example\": \"standard\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"Location where the error occurred (e.g., query, path, body)\",\n            \"example\": \"example-value\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"description\": \"Additional context about the specific error\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\"\
  : \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-analytics-events-error-schema.json
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
