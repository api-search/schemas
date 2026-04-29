---
description: ''
layout: schema
name: UpdateCredentialRequest
properties_list:
- description: ''
  name: externalCredential
  type: string
- description: ''
  name: authenticationProtocol
  type: string
- description: ''
  name: principalName
  type: string
- description: ''
  name: principalType
  type: string
- description: ''
  name: credentials
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-update-credential-request-schema.json
slug: salesforce-update-credential-request
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"externalCredential\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"authenticationProtocol\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principalName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principalType\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"credentials\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"testCredential\": {\n          \"type\": \"object\",\n          \"properties\": {\n            \"value\": {\n              \"type\": \"string\",\n              \"example\": \"example_value\"\n            },\n            \"encrypted\": {\n              \"type\": \"boolean\",\n              \"example\": true\n            }\n          },\n          \"required\": [\n            \"value\",\n            \"encrypted\"\n          ]\n   \
  \     }\n      },\n      \"required\": [\n        \"testCredential\"\n      ]\n    }\n  },\n  \"required\": [\n    \"externalCredential\",\n    \"authenticationProtocol\",\n    \"principalName\",\n    \"principalType\",\n    \"credentials\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"UpdateCredentialRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-update-credential-request-schema.json
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
title: UpdateCredentialRequest
---
