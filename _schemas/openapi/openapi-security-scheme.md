---
description: Defines a security scheme that can be used by the operations.
layout: schema
name: OpenAPI Security Scheme Object
properties_list:
- description: The type of the security scheme.
  name: type
  type: string
- description: A description for the security scheme.
  name: description
  type: string
- description: The name of the header, query, or cookie parameter to be used (required for apiKey).
  name: name
  type: string
- description: The location of the API key (required for apiKey).
  name: in
  type: string
- description: The name of the HTTP Authorization scheme (required for http).
  name: scheme
  type: string
- description: A hint to the client to identify how the bearer token is formatted.
  name: bearerFormat
  type: string
- description: ''
  name: flows
  type: object
- description: OpenId Connect URL to discover OAuth2 configuration values (required for openIdConnect).
  name: openIdConnectUrl
  type: string
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-security-scheme.json
slug: openapi-security-scheme
source_filename: openapi-security-scheme.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-security-scheme.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI Security Scheme Object\",\n  \"description\": \"Defines a security scheme that can be used by the operations.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"type\"\n  ],\n  \"properties\": {\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the security scheme.\",\n      \"enum\": [\n        \"apiKey\",\n        \"http\",\n        \"mutualTLS\",\n        \"oauth2\",\n        \"openIdConnect\"\n      ]\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"A description for the security scheme.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the header, query, or cookie parameter to be used (required for apiKey).\"\n    },\n    \"in\": {\n      \"type\": \"string\",\n      \"description\": \"The location of the API key (required\
  \ for apiKey).\",\n      \"enum\": [\n        \"query\",\n        \"header\",\n        \"cookie\"\n      ]\n    },\n    \"scheme\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the HTTP Authorization scheme (required for http).\"\n    },\n    \"bearerFormat\": {\n      \"type\": \"string\",\n      \"description\": \"A hint to the client to identify how the bearer token is formatted.\"\n    },\n    \"flows\": {\n      \"$ref\": \"openapi-oauth-flows.json\"\n    },\n    \"openIdConnectUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"OpenId Connect URL to discover OAuth2 configuration values (required for openIdConnect).\"\n    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-security-scheme.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI Security Scheme Object
---
