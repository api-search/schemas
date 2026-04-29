---
description: ''
layout: schema
name: ClientInfo
properties_list:
- description: ''
  name: applicationName
  type: string
- description: ''
  name: applicationUrl
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-client-info-schema.json
slug: salesforce-client-info
source_filename: salesforce-client-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"applicationName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"applicationUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"applicationName\",\n    \"applicationUrl\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClientInfo\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-client-info-schema.json
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
title: ClientInfo
---
