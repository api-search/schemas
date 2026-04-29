---
description: ''
layout: schema
name: SuccessfulJWTBearerTokenFlow
properties_list:
- description: ''
  name: access_token
  type: string
- description: ''
  name: scope
  type: string
- description: ''
  name: instance_url
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: token_type
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-jwt-bearer-token-flow-schema.json
slug: salesforce-successful-jwt-bearer-token-flow
source_filename: salesforce-successful-jwt-bearer-token-flow-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"instance_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    }\n  },\n  \"required\": [\n    \"access_token\",\n    \"scope\",\n    \"instance_url\",\n    \"id\",\n    \"token_type\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulJWTBearerTokenFlow\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-jwt-bearer-token-flow-schema.json
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
title: SuccessfulJWTBearerTokenFlow
---
