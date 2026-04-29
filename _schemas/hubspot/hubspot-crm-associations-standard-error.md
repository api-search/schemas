---
description: Standard error in batch operations
layout: schema
name: StandardError
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
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-standard-error-schema.json
slug: hubspot-crm-associations-standard-error
source_filename: hubspot-crm-associations-standard-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Standard error in batch operations\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"This is an example description.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"code\": \"example-value\",\n          \"subCategory\": \"standard\",\n          \"in\": \"example-value\",\n          \"context\": {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Details about a specific error\",\n        \"properties\": {\n          \"\
  message\": {\n            \"type\": \"string\",\n            \"example\": \"This is an example description.\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"example\": \"standard\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"example\": \"example-value\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"key\": \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"category\"\
  ,\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StandardError\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-standard-error-schema.json
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
title: StandardError
---
