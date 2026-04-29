---
description: ''
layout: schema
name: RelatedNamedCredential
properties_list:
- description: ''
  name: developerName
  type: string
- description: ''
  name: id
  type: string
- description: ''
  name: masterLabel
  type: string
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-related-named-credential-schema.json
slug: salesforce-related-named-credential
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"developerName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"masterLabel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"developerName\",\n    \"id\",\n    \"masterLabel\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RelatedNamedCredential\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-related-named-credential-schema.json
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
title: RelatedNamedCredential
---
