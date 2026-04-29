---
description: ''
layout: schema
name: SuccessfulRefreshToken
properties_list:
- description: ''
  name: access_token
  type: string
- description: ''
  name: signature
  type: string
- description: ''
  name: scope
  type: string
- description: ''
  name: id_token
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
- description: ''
  name: issued_at
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-refresh-token-schema.json
slug: salesforce-successful-refresh-token
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"signature\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id_token\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"instance_url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"issued_at\": {\n      \"type\": \"string\",\n      \"example\": \"2026-01-15T10:30:00Z\"\n    }\n  },\n  \"required\": [\n    \"access_token\",\n    \"signature\",\n    \"scope\",\n    \"id_token\",\n    \"instance_url\",\n    \"id\",\n    \"token_type\",\n    \"issued_at\"\n\
  \  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulRefreshToken\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-refresh-token-schema.json
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
title: SuccessfulRefreshToken
---
