---
description: Details about a specific error
layout: schema
name: ErrorDetail
properties_list:
- description: ''
  name: message
  type: string
- description: ''
  name: code
  type: string
- description: ''
  name: subCategory
  type: string
- description: ''
  name: in
  type: string
- description: ''
  name: context
  type: object
provider_name: HubSpot
provider_slug: hubspot
schema_file: json-schema/hubspot-crm-associations-error-detail-schema.json
slug: hubspot-crm-associations-error-detail
source_filename: hubspot-crm-associations-error-detail-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"description\": \"Details about a specific error\",\n  \"properties\": {\n    \"message\": {\n      \"type\": \"string\",\n      \"example\": \"This is an example description.\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"subCategory\": {\n      \"type\": \"string\",\n      \"example\": \"standard\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"example\": \"example-value\"\n    },\n    \"context\": {\n      \"type\": \"object\",\n      \"example\": {\n        \"key\": \"value\"\n      }\n    }\n  },\n  \"required\": [\n    \"message\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ErrorDetail\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/hubspot/refs/heads/main/json-schema/hubspot-crm-associations-error-detail-schema.json
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
