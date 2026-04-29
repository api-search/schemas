---
description: ''
layout: schema
name: Location
properties_list:
- description: ''
  name: column
  type: integer
- description: ''
  name: line
  type: integer
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-location-schema.json
slug: salesforce-location
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"column\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    },\n    \"line\": {\n      \"type\": \"integer\",\n      \"example\": 10\n    }\n  },\n  \"required\": [\n    \"column\",\n    \"line\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Location\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-location-schema.json
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
title: Location
---
