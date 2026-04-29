---
description: Error response
layout: schema
name: Error
properties_list:
- description: The error category
  name: category
  type: string
- description: Unique request identifier for debugging
  name: correlationId
  type: string
- description: Human-readable error message
  name: message
  type: string
- description: More specific error category
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
schema_file: json-schema/hubspot-engagement-notes-error-schema.json
slug: hubspot-engagement-notes-error
source_filename: hubspot-engagement-notes-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Error response\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The error category\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"Unique request identifier for debugging\",\n      \"format\": \"uuid\",\n      \"example\": \"aeb5f871-7f07-4993-9211-075dc63e7cbf\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Human-readable error message\",\n      \"example\": \"Invalid input (details will vary based on the error)\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"More specific error category\",\n      \"example\": \"standard\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"example\": {\n\
  \        \"key\": \"value\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"code\": \"example-value\",\n          \"in\": \"example-value\",\n          \"subCategory\": \"standard\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed error information\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Error message\",\n            \"example\": \"This is an example description.\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"Error code\",\n            \"example\": \"example-value\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"Field where error occurred\",\n\
  \            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"Error subcategory\",\n            \"example\": \"standard\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-error-schema.json
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
