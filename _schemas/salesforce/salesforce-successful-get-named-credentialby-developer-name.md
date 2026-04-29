---
description: ''
layout: schema
name: SuccessfulGetNamedCredentialbyDeveloperName
properties_list:
- description: ''
  name: calloutOptions
  type: object
- description: ''
  name: calloutUrl
  type: string
- description: ''
  name: customHeaders
  type: array
- description: ''
  name: developerName
  type: string
- description: ''
  name: externalCredentials
  type: array
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
  name: type
  type: string
- description: ''
  name: url
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-get-named-credentialby-developer-name-schema.json
slug: salesforce-successful-get-named-credentialby-developer-name
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"calloutOptions\": {\n      \"type\": \"object\",\n      \"properties\": {\n        \"allowMergeFieldsInBody\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"allowMergeFieldsInHeader\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        },\n        \"generateAuthorizationHeader\": {\n          \"type\": \"boolean\",\n          \"example\": true\n        }\n      },\n      \"required\": [\n        \"allowMergeFieldsInBody\",\n        \"allowMergeFieldsInHeader\",\n        \"generateAuthorizationHeader\"\n      ]\n    },\n    \"calloutUrl\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    },\n    \"customHeaders\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"developerName\": {\n      \"type\": \"string\",\n    \
  \  \"example\": \"example_value\"\n    },\n    \"externalCredentials\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"developerName\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"id\": {\n            \"type\": \"string\",\n            \"example\": \"abc123\"\n          },\n          \"masterLabel\": {\n            \"type\": \"string\",\n            \"example\": \"example_value\"\n          },\n          \"url\": {\n            \"type\": \"string\",\n            \"example\": \"https://www.example.com\"\n          }\n        },\n        \"required\": [\n          \"developerName\",\n          \"id\",\n          \"masterLabel\",\n          \"url\"\n        ]\n      }\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"example\": \"abc123\"\n    },\n    \"masterLabel\": {\n      \"type\": \"\
  string\",\n      \"example\": \"example_value\"\n    },\n    \"parameters\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"example\": \"https://www.example.com\"\n    }\n  },\n  \"required\": [\n    \"calloutOptions\",\n    \"calloutUrl\",\n    \"customHeaders\",\n    \"developerName\",\n    \"externalCredentials\",\n    \"id\",\n    \"masterLabel\",\n    \"parameters\",\n    \"type\",\n    \"url\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulGetNamedCredentialbyDeveloperName\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-get-named-credentialby-developer-name-schema.json
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
title: SuccessfulGetNamedCredentialbyDeveloperName
---
