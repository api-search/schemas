---
description: Detailed error information
layout: schema
name: ErrorDetail
properties_list:
- description: The error message
  name: message
  type: string
- description: An error code
  name: code
  type: string
- description: The location of the error
  name: in
  type: string
- description: A specific error subcategory
  name: subCategory
  type: string
- description: ''
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-custom-workflow-actions-error-detail-schema.json
slug: hubspot-custom-workflow-actions-error-detail
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed error information\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"The error message\",\n      \"example\": \"This is an example description.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"An error code\",\n      \"example\": \"example-value\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the error\",\n      \"example\": \"example-value\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"A specific error subcategory\",\n      \"example\": \"standard\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-custom-workflow-actions-error-detail-schema.json
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
