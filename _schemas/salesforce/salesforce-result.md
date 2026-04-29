---
description: ''
layout: schema
name: Result
properties_list:
- description: ''
  name: referenceId
  type: string
- description: ''
  name: id
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-result-schema.json
slug: salesforce-result
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"referenceId\": {\n      \"type\": \"string\",\n      \"example\": \"500123\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    }\n  },\n  \"required\": [\n    \"referenceId\",\n    \"id\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Result\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-result-schema.json
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
title: Result
---
