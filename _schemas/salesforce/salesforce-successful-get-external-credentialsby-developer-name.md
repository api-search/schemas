---
description: ''
layout: schema
name: SuccessfulGetExternalCredentialsbyDeveloperName
properties_list:
- description: ''
  name: authenticationProtocol
  type: string
- description: ''
  name: authenticationProtocolVariant
  type: string
- description: ''
  name: authenticationStatus
  type: string
- description: ''
  name: customHeaders
  type: array
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
  name: parameters
  type: array
- description: ''
  name: principals
  type: array
- description: ''
  name: relatedNamedCredentials
  type: array
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-get-external-credentialsby-developer-name-schema.json
slug: salesforce-successful-get-external-credentialsby-developer-name
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"authenticationProtocol\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"authenticationProtocolVariant\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"authenticationStatus\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"customHeaders\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"developerName\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"masterLabel\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"\
  string\"\n      }\n    },\n    \"principals\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"relatedNamedCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"developerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"masterLabel\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          }\n        },\n        \"required\": [\n          \"developerName\",\n          \"id\",\n          \"masterLabel\",\n          \"\
  url\"\n        ]\n      }\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"authenticationProtocol\",\n    \"authenticationProtocolVariant\",\n    \"authenticationStatus\",\n    \"customHeaders\",\n    \"developerName\",\n    \"id\",\n    \"masterLabel\",\n    \"parameters\",\n    \"principals\",\n    \"relatedNamedCredentials\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulGetExternalCredentialsbyDeveloperName\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-get-external-credentialsby-developer-name-schema.json
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
title: SuccessfulGetExternalCredentialsbyDeveloperName
---
