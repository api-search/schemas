---
description: An error response
layout: schema
name: Error
properties_list:
- description: The error category
  name: category
  type: string
- description: A unique identifier for this error instance
  name: correlationId
  type: string
- description: A human-readable error message
  name: message
  type: string
- description: A more specific error category
  name: subCategory
  type: string
- description: Detailed error information
  name: errors
  type: array
- description: Additional context about the error
  name: context
  type: object
- description: Related links
  name: links
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-error-schema.json
slug: hubspot-custom-workflow-actions-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An error response\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The error category\",\n      \"example\": \"standard\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for this error instance\",\n      \"format\": \"uuid\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable error message\",\n      \"example\": \"This is an example description.\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"A more specific error category\",\n      \"example\": \"standard\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed error information\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n      \
  \    \"code\": \"example-value\",\n          \"in\": \"example-value\",\n          \"subCategory\": \"standard\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed error information\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"The error message\",\n            \"example\": \"This is an example description.\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"An error code\",\n            \"example\": \"example-value\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"The location of the error\",\n            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"A specific error subcategory\"\
  ,\n            \"example\": \"standard\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the error\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Related links\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-error-schema.json
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
