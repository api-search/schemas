---
description: ''
layout: schema
name: CreateNamedCredentialRequest
properties_list:
- description: ''
  name: developerName
  type: string
- description: ''
  name: masterLabel
  type: string
- description: ''
  name: type
  type: string
- description: ''
  name: calloutUrl
  type: string
- description: ''
  name: externalCredentials
  type: array
- description: ''
  name: customHeaders
  type: array
- description: ''
  name: calloutOptions
  type: object
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-create-named-credential-request-schema.json
slug: salesforce-create-named-credential-request
source_filename: salesforce-create-named-credential-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"developerName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"masterLabel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"calloutUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"externalCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"developerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          }\n        },\n        \"required\": [\n          \"developerName\"\n        ]\n      }\n    },\n    \"customHeaders\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n\
  \        \"type\": \"object\",\n        \"properties\": {\n          \"headerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"headerValue\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"sequenceNumber\": {\n            \"type\": \"integer\",\n            \"example\": 10\n          }\n        },\n        \"required\": [\n          \"headerName\",\n          \"headerValue\",\n          \"sequenceNumber\"\n        ]\n      }\n    },\n    \"calloutOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"allowMergeFieldsInBody\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"allowMergeFieldsInHeader\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"generateAuthorizationHeader\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n     \
  \ },\n      \"required\": [\n        \"allowMergeFieldsInBody\",\n        \"allowMergeFieldsInHeader\",\n        \"generateAuthorizationHeader\"\n      ]\n    }\n  },\n  \"required\": [\n    \"developerName\",\n    \"masterLabel\",\n    \"type\",\n    \"calloutUrl\",\n    \"externalCredentials\",\n    \"customHeaders\",\n    \"calloutOptions\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CreateNamedCredentialRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-create-named-credential-request-schema.json
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
title: CreateNamedCredentialRequest
---
