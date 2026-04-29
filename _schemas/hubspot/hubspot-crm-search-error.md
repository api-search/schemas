---
description: An error response.
layout: schema
name: Error
properties_list:
- description: ''
  name: status
  type: string
- description: ''
  name: message
  type: string
- description: ''
  name: correlationId
  type: string
- description: ''
  name: category
  type: string
- description: ''
  name: errors
  type: array
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-search-error-schema.json
slug: hubspot-crm-search-error
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"An error response.\",\n  \"properties\": {\n    \"status\": {\n      \"type\": \"string\",\n      \"example\": \"active\"\n    },\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"This is an example description.\"\n    },\n    \"correlationId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"category\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"errors\": {\n      \"type\": \"array\",\n      \"example\": [\n        {\n          \"message\": \"This is an example description.\",\n          \"in\": \"example-value\",\n          \"code\": \"example-value\"\n        }\n      ],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"message\": {\n            \"type\": \"string\"\n          },\n          \"in\": {\n            \"type\": \"string\"\n          },\n          \"code\": {\n            \"type\": \"string\"\
  \n          }\n        }\n      }\n    }\n  },\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Error\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-search-error-schema.json
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
