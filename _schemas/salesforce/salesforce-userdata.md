---
description: ''
layout: schema
name: Userdata
properties_list:
- description: ''
  name: firstName
  type: string
- description: ''
  name: lastName
  type: string
- description: ''
  name: email
  type: string
- description: ''
  name: username
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-userdata-schema.json
slug: salesforce-userdata
source_filename: salesforce-userdata-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"firstName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"lastName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"email\": {\n      \"type\": \"string\",\n      \"example\": \"user@example.com\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"firstName\",\n    \"lastName\",\n    \"email\",\n    \"username\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Userdata\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-userdata-schema.json
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
title: Userdata
---
