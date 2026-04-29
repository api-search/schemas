---
description: Error information for a batch operation item
layout: schema
name: BatchError
properties_list:
- description: The error status
  name: status
  type: string
- description: The error category
  name: category
  type: string
- description: The error message
  name: message
  type: string
- description: ''
  name: context
  type: object
- description: ''
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-engagement-notes-batch-error-schema.json
slug: hubspot-engagement-notes-batch-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Error information for a batch operation item\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The error status\",\n      \"example\": \"error\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The error category\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The error message\",\n      \"example\": \"Property value is invalid\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"code\": \"example-value\",\n          \"in\": \"example-value\",\n          \"subCategory\": \"standard\",\n          \"context\": {\n            \"key\": \"value\"\n\
  \          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed error information\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Error message\",\n            \"example\": \"This is an example description.\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"Error code\",\n            \"example\": \"example-value\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"Field where error occurred\",\n            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"Error subcategory\",\n            \"example\": \"standard\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"key\": \"value\"\n          \
  \  }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BatchError\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-engagement-notes-batch-error-schema.json
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
title: BatchError
---
