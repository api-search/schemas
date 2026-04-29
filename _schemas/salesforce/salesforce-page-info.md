---
description: ''
layout: schema
name: PageInfo
properties_list:
- description: ''
  name: hasNextPage
  type: boolean
- description: ''
  name: hasPreviousPage
  type: boolean
- description: ''
  name: startCursor
  type: string
- description: ''
  name: endCursor
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-page-info-schema.json
slug: salesforce-page-info
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"hasNextPage\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"hasPreviousPage\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"startCursor\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"endCursor\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"hasNextPage\",\n    \"hasPreviousPage\",\n    \"startCursor\",\n    \"endCursor\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PageInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-page-info-schema.json
tags:
- AI
- Analytics
- Cloud
- Commerce
- CRM
- Customer Service
- Enterprise
- Marketing
- Platform
- Sales
title: PageInfo
---
