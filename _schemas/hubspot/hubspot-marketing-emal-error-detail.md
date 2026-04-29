---
description: Detailed error information
layout: schema
name: ErrorDetail
properties_list:
- description: Error message
  name: message
  type: string
- description: Error code
  name: code
  type: string
- description: Field where error occurred
  name: in
  type: string
- description: Error subcategory
  name: subCategory
  type: string
- description: ''
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-marketing-emal-error-detail-schema.json
slug: hubspot-marketing-emal-error-detail
source_filename: hubspot-marketing-emal-error-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Detailed error information\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"description\": \"Error message\",\n      \"example\": \"This is an example description.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"Error code\",\n      \"example\": \"example-value\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"Field where error occurred\",\n      \"example\": \"example-value\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"description\": \"Error subcategory\",\n      \"example\": \"standard\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-marketing-emal-error-detail-schema.json
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
