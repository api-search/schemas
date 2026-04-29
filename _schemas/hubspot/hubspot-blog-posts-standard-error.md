---
description: Standard error in batch operations
layout: schema
name: StandardError
properties_list:
- description: Error status
  name: status
  type: string
- description: ID of the failed item
  name: id
  type: string
- description: Error category
  name: category
  type: string
- description: Error message
  name: message
  type: string
- description: Detailed errors
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
schema_file: json-schema/hubspot-blog-posts-standard-error-schema.json
slug: hubspot-blog-posts-standard-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Standard error in batch operations\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"Error status\",\n      \"example\": \"active\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"ID of the failed item\",\n      \"example\": \"500123\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"description\": \"Error category\",\n      \"example\": \"standard\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"This is an example description.\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"description\": \"Detailed errors\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"code\": \"example-value\",\n          \"subCategory\": \"standard\",\n          \"in\": \"example-value\",\n          \"context\"\
  : {\n            \"key\": \"value\"\n          }\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"description\": \"Detailed error information\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\",\n            \"description\": \"Error message\",\n            \"example\": \"This is an example description.\"\n          },\n          \"code\": {\n            \"type\": \"string\",\n            \"description\": \"Error code\",\n            \"example\": \"example-value\"\n          },\n          \"subCategory\": {\n            \"type\": \"string\",\n            \"description\": \"Error subcategory\",\n            \"example\": \"standard\"\n          },\n          \"in\": {\n            \"type\": \"string\",\n            \"description\": \"Location of error\",\n            \"example\": \"example-value\"\n          },\n          \"context\": {\n            \"type\": \"object\",\n            \"example\": {\n              \"key\"\
  : \"value\"\n            }\n          }\n        },\n        \"required\": [\n          \"message\"\n        ]\n      }\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    },\n    \"links\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"status\",\n    \"category\",\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StandardError\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-blog-posts-standard-error-schema.json
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
