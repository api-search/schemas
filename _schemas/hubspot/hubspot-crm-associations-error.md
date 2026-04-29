---
description: Standard error response
layout: schema
name: Error
properties_list:
- description: ''
  name: category
  type: string
- description: ''
  name: correlationId
  type: string
- description: ''
  name: message
  type: string
- description: ''
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
schema_file: json-schema/hubspot-crm-associations-error-schema.json
slug: hubspot-crm-associations-error
source_filename: hubspot-crm-associations-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Standard error response\",\n  \"properties\": {\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"VALIDATION_ERROR\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"format\": \"uuid\",\n      \"example\": \"a1b2c3d4-e5f6-7890-abcd-ef1234567890\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"This is an example description.\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"code\": \"example-value\",\n          \"subCategory\"\
  : \"standard\",\n          \"in\": \"example-value\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Details about a specific error\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"example\": \"This is an example description.\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"example\": \"example-value\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n     \
  \ }\n    }\n  },\n  \"required\": [\n    \"category\",\n    \"correlationId\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-error-schema.json
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
