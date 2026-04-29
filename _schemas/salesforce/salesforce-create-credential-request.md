---
description: ''
layout: schema
name: CreateCredentialRequest
properties_list:
- description: ''
  name: authenticationProtocol
  type: string
- description: ''
  name: credentials
  type: object
- description: ''
  name: externalCredential
  type: string
- description: ''
  name: principalName
  type: string
- description: ''
  name: principalType
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-credential-request-schema.json
slug: salesforce-create-credential-request
source_filename: salesforce-create-credential-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationProtocol\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"credentials\": {\n      \"type\": \"object\",\n      \"example\": \"example_value\"\n    },\n    \"externalCredential\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principalName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"authenticationProtocol\",\n    \"credentials\",\n    \"externalCredential\",\n    \"principalName\",\n    \"principalType\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateCredentialRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-credential-request-schema.json
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
title: CreateCredentialRequest
---
