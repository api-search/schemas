---
description: ''
layout: schema
name: OpenIDConnectDynamicClientRegistrationEndpointRequest
properties_list:
- description: ''
  name: redirect_uris
  type: array
- description: ''
  name: response_types
  type: array
- description: ''
  name: grant_types
  type: array
- description: ''
  name: application_type
  type: string
- description: ''
  name: contacts
  type: array
- description: ''
  name: client_name
  type: string
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-open-id-connect-dynamic-client-registration-endpoint-request-schema.json
slug: salesforce-open-id-connect-dynamic-client-registration-endpoint-request
source_filename: salesforce-open-id-connect-dynamic-client-registration-endpoint-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"redirect_uris\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"response_types\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"grant_types\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"application_type\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"contacts\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"client_name\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"redirect_uris\"\
  ,\n    \"response_types\",\n    \"grant_types\",\n    \"application_type\",\n    \"contacts\",\n    \"client_name\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenIDConnectDynamicClientRegistrationEndpointRequest\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-open-id-connect-dynamic-client-registration-endpoint-request-schema.json
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
title: OpenIDConnectDynamicClientRegistrationEndpointRequest
---
