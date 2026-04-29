---
description: An error from a batch operation
layout: schema
name: BatchError
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: errors
  type: array
- description: ''
  name: context
  type: object
- description: ''
  name: links
  type: object
- description: ''
  name: subCategory
  type: string
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/commerce-payments-api-batch-error-schema.json
slug: commerce-payments-api-batch-error
source_filename: commerce-payments-api-batch-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-error-schema.json\",\n  \"title\": \"BatchError\",\n  \"description\": \"An error from a batch operation\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"This is an example description.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed error information\",\n        \"required\": [\n          \"message\"\n        ],\n        \"properties\": {\n          \"message\"\
  : {\n            \"type\": \"string\",\n            \"description\": \"The error message\",\n            \"example\": \"This is an example description.\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"An error code\",\n            \"example\": \"example-value\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"The location of the error\",\n            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"A specific error subcategory\",\n            \"example\": \"standard\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"additionalProperties\": {\n              \"type\": \"array\",\n              \"items\": {\n                \"type\": \"string\"\n              }\n            },\n            \"example\": {\n              \"key\": \"value\"\n         \
  \   }\n          }\n        }\n      },\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"code\": \"example-value\",\n          \"in\": \"example-value\",\n          \"subCategory\": \"standard\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ]\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"array\",\n        \"items\": {\n          \"type\": \"string\"\n        }\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      },\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"message\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/commerce-payments-api-batch-error-schema.json
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
