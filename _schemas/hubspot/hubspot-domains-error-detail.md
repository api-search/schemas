---
description: Detailed information about a specific error
layout: schema
name: ErrorDetail
properties_list:
- description: A human-readable message describing the specific error
  name: message
  type: string
- description: An error code for this specific error
  name: code
  type: string
- description: The field or parameter where the error occurred
  name: in
  type: string
- description: A specific subcategory for this error
  name: subCategory
  type: string
- description: Additional context for this error
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-domains-error-detail-schema.json
slug: hubspot-domains-error-detail
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed information about a specific error\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable message describing the specific error\",\n      \"example\": \"This is an example description.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"An error code for this specific error\",\n      \"example\": \"example-value\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"The field or parameter where the error occurred\",\n      \"example\": \"example-value\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"A specific subcategory for this error\",\n      \"example\": \"standard\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"description\": \"Additional context for this error\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n \
  \ \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-domains-error-detail-schema.json
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
title: ErrorDetail
---
