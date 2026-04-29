---
description: ''
layout: schema
name: SuccessfulOpenIDConnectDiscoveryEndpoint
properties_list:
- description: ''
  name: end_session_endpoint
  type: string
- description: ''
  name: frontchannel_logout_supported
  type: boolean
- description: ''
  name: frontchannel_logout_session_supported
  type: boolean
- description: ''
  name: issuer
  type: string
- description: ''
  name: authorization_endpoint
  type: string
- description: ''
  name: token_endpoint
  type: string
- description: ''
  name: revocation_endpoint
  type: string
- description: ''
  name: userinfo_endpoint
  type: string
- description: ''
  name: jwks_uri
  type: string
- description: ''
  name: registration_endpoint
  type: string
- description: ''
  name: introspection_endpoint
  type: string
- description: ''
  name: scopes_supported
  type: array
- description: ''
  name: response_types_supported
  type: array
- description: ''
  name: subject_types_supported
  type: array
- description: ''
  name: id_token_signing_alg_values_supported
  type: array
- description: ''
  name: display_values_supported
  type: array
- description: ''
  name: token_endpoint_auth_methods_supported
  type: array
- description: ''
  name: claims_supported
  type: array
provider_name: Salesforce
provider_slug: salesforce
schema_file: json-schema/salesforce-successful-open-id-connect-discovery-endpoint-schema.json
slug: salesforce-successful-open-id-connect-discovery-endpoint
source_filename: salesforce-successful-open-id-connect-discovery-endpoint-schema.json
source_heading: JSON Schema
source_json: "{\n  \"type\": \"object\",\n  \"properties\": {\n    \"end_session_endpoint\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"frontchannel_logout_supported\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"frontchannel_logout_session_supported\": {\n      \"type\": \"boolean\",\n      \"example\": true\n    },\n    \"issuer\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"authorization_endpoint\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"token_endpoint\": {\n      \"type\": \"string\",\n      \"example\": \"CAUQAA\"\n    },\n    \"revocation_endpoint\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"userinfo_endpoint\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"jwks_uri\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"\
  registration_endpoint\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"introspection_endpoint\": {\n      \"type\": \"string\",\n      \"example\": \"example_value\"\n    },\n    \"scopes_supported\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"response_types_supported\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"subject_types_supported\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"id_token_signing_alg_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"CAUQAA\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"display_values_supported\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"token_endpoint_auth_methods_supported\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": \"CAUQAA\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"claims_supported\": {\n      \"type\": \"array\",\n      \"description\": \"\",\n      \"example\": [],\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"end_session_endpoint\",\n    \"frontchannel_logout_supported\",\n    \"frontchannel_logout_session_supported\",\n    \"issuer\",\n    \"authorization_endpoint\",\n    \"token_endpoint\",\n    \"revocation_endpoint\",\n    \"userinfo_endpoint\",\n    \"jwks_uri\",\n    \"registration_endpoint\",\n    \"introspection_endpoint\",\n    \"scopes_supported\",\n    \"response_types_supported\",\n    \"subject_types_supported\",\n    \"\
  id_token_signing_alg_values_supported\",\n    \"display_values_supported\",\n    \"token_endpoint_auth_methods_supported\",\n    \"claims_supported\"\n  ],\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SuccessfulOpenIDConnectDiscoveryEndpoint\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/salesforce/refs/heads/main/json-schema/salesforce-successful-open-id-connect-discovery-endpoint-schema.json
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
title: SuccessfulOpenIDConnectDiscoveryEndpoint
---
