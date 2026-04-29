---
description: Represents an error response from the API
layout: schema
name: Error
properties_list:
- description: The error category
  name: category
  type: string
- description: A unique identifier for the request, useful for debugging
  name: correlationId
  type: string
- description: A human-readable message describing the error
  name: message
  type: string
- description: A more specific category for the error
  name: subCategory
  type: string
- description: Additional context about the error
  name: context
  type: object
- description: Links to documentation or remediation steps
  name: links
  type: object
- description: A list of specific error details
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-domains-error-schema.json
slug: hubspot-domains-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Represents an error response from the API\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"The error category\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"description\": \"A unique identifier for the request, useful for debugging\",\n      \"format\": \"uuid\",\n      \"example\": \"aeb5f871-7f07-4993-9211-075dc63e7cbf\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable message describing the error\",\n      \"example\": \"Invalid input (details will vary based on the error)\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"A more specific category for the error\",\n      \"example\": \"standard\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context about the error\",\n\
  \      \"example\": {\n        \"missingScopes\": [\n          \"scope1\",\n          \"scope2\"\n        ]\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"description\": \"Links to documentation or remediation steps\",\n      \"example\": {\n        \"knowledge-base\": \"https://www.hubspot.com/products/service/knowledge-base\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"A list of specific error details\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"code\": \"example-value\",\n          \"in\": \"example-value\",\n          \"subCategory\": \"standard\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed information about a specific error\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\"\
  ,\n            \"description\": \"A human-readable message describing the specific error\",\n            \"example\": \"This is an example description.\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"An error code for this specific error\",\n            \"example\": \"example-value\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"The field or parameter where the error occurred\",\n            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"A specific subcategory for this error\",\n            \"example\": \"standard\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"description\": \"Additional context for this error\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\":\
  \ [\n          \"message\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-domains-error-schema.json
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
