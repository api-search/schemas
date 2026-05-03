---
description: Schema describing the structure of an OAuth 2.0 error response as defined in RFC 6749 Section 5.2. The authorization server responds with an HTTP 400 (Bad Request) status code and includes a JSON body with error details.
layout: schema
name: OAuth 2.0 Error Response
properties_list:
- description: A single ASCII error code from the defined set of error codes.
  name: error
  type: string
- description: A human-readable ASCII text providing additional information, used to assist the client developer in understanding the error that occurred.
  name: error_description
  type: string
- description: A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error.
  name: error_uri
  type: string
provider_name: OAuth
provider_slug: oauth
schema_file: json-schema/oauth-error-response.json
slug: oauth-error-response
source_filename: oauth-error-response.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"oauth-error-response.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OAuth 2.0 Error Response\",\n  \"description\": \"Schema describing the structure of an OAuth 2.0 error response as defined in RFC 6749 Section 5.2. The authorization server responds with an HTTP 400 (Bad Request) status code and includes a JSON body with error details.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"error\"\n  ],\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"description\": \"A single ASCII error code from the defined set of error codes.\",\n      \"enum\": [\n        \"invalid_request\",\n        \"invalid_client\",\n        \"invalid_grant\",\n        \"unauthorized_client\",\n        \"unsupported_grant_type\",\n        \"invalid_scope\",\n        \"unsupported_token_type\"\n      ]\n    },\n    \"error_description\": {\n      \"type\": \"string\",\n      \"description\": \"A human-readable ASCII\
  \ text providing additional information, used to assist the client developer in understanding the error that occurred.\",\n      \"pattern\": \"^[\\\\x20-\\\\x21\\\\x23-\\\\x5B\\\\x5D-\\\\x7E]*$\"\n    },\n    \"error_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"A URI identifying a human-readable web page with information about the error, used to provide the client developer with additional information about the error.\"\n    }\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oauth/refs/heads/main/json-schema/oauth-error-response.json
tags:
- Access Control
- Authorization
- OAuth
- Security
- Tokens
title: OAuth 2.0 Error Response
---
