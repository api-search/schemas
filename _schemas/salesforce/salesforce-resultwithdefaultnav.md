---
description: ''
layout: schema
name: Resultwithdefaultnav
properties_list:
- description: ''
  name: currentPageUrl
  type: string
- description: ''
  name: eTag
  type: string
- description: ''
  name: navItems
  type: array
- description: ''
  name: nextPageUrl
  type: '[''string'', ''null'']'
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-resultwithdefaultnav-schema.json
slug: salesforce-resultwithdefaultnav
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"currentPageUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"eTag\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"navItems\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"nextPageUrl\": {\n      \"type\": \"['string', 'null']\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"currentPageUrl\",\n    \"eTag\",\n    \"navItems\",\n    \"nextPageUrl\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Resultwithdefaultnav\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-resultwithdefaultnav-schema.json
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
title: Resultwithdefaultnav
---
