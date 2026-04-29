---
description: ''
layout: schema
name: CreateExternalCredentialRequest
properties_list:
- description: ''
  name: developerName
  type: string
- description: ''
  name: masterLabel
  type: string
- description: ''
  name: authenticationProtocol
  type: string
- description: ''
  name: principals
  type: array
- description: ''
  name: customHeaders
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-external-credential-request-schema.json
slug: salesforce-create-external-credential-request
source_filename: salesforce-create-external-credential-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"developerName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"masterLabel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"authenticationProtocol\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"principals\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"principalName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"principalType\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"sequenceNumber\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n        },\n        \"required\": [\n          \"principalName\",\n          \"principalType\"\
  ,\n          \"sequenceNumber\"\n        ]\n      }\n    },\n    \"customHeaders\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"headerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"headerValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"sequenceNumber\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n        },\n        \"required\": [\n          \"headerName\",\n          \"headerValue\",\n          \"sequenceNumber\"\n        ]\n      }\n    }\n  },\n  \"required\": [\n    \"developerName\",\n    \"masterLabel\",\n    \"authenticationProtocol\",\n    \"principals\",\n    \"customHeaders\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateExternalCredentialRequest\"\
  \n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-external-credential-request-schema.json
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
title: CreateExternalCredentialRequest
---
