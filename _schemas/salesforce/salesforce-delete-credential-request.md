---
description: ''
layout: schema
name: DeleteCredentialRequest
properties_list:
- description: ''
  name: externalCredential
  type: string
- description: ''
  name: principalType
  type: string
- description: ''
  name: principalName
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-delete-credential-request-schema.json
slug: salesforce-delete-credential-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalCredential\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principalName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"externalCredential\",\n    \"principalType\",\n    \"principalName\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DeleteCredentialRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-delete-credential-request-schema.json
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
title: DeleteCredentialRequest
---
