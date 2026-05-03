---
description: Schema describing the structure of a successful OAuth 2.0 access token response as defined in RFC 6749 Section 5.1. The authorization server issues an access token and optional refresh token upon a valid and authorized token request.
layout: schema
name: OAuth 2.0 Token Response
properties_list:
- description: The access token issued by the authorization server.
  name: access_token
  type: string
- description: The type of the token issued as described in RFC 6749 Section 7.1. Value is case insensitive.
  name: token_type
  type: string
- description: The lifetime in seconds of the access token. If omitted, the authorization server SHOULD provide the expiration time via other means or document the default value.
  name: expires_in
  type: integer
- description: The refresh token, which can be used to obtain new access tokens using the same authorization grant.
  name: refresh_token
  type: string
- description: The scope of the access token as a space-delimited list of case-sensitive strings. OPTIONAL if identical to the scope requested; otherwise, REQUIRED.
  name: scope
  type: string
provider_name: OAuth
provider_slug: oauth
schema_file: json-schema/oauth-token-response.json
slug: oauth-token-response
source_filename: oauth-token-response.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"oauth-token-response.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OAuth 2.0 Token Response\",\n  \"description\": \"Schema describing the structure of a successful OAuth 2.0 access token response as defined in RFC 6749 Section 5.1. The authorization server issues an access token and optional refresh token upon a valid and authorized token request.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"access_token\",\n    \"token_type\"\n  ],\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"The access token issued by the authorization server.\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the token issued as described in RFC 6749 Section 7.1. Value is case insensitive.\",\n      \"examples\": [\n        \"Bearer\",\n        \"mac\"\n      ]\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"The lifetime in seconds of the access token. If omitted, the authorization server SHOULD provide the expiration time via other means or document the default value.\",\n      \"minimum\": 0,\n      \"examples\": [\n        3600\n      ]\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"The refresh token, which can be used to obtain new access tokens using the same authorization grant.\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope of the access token as a space-delimited list of case-sensitive strings. OPTIONAL if identical to the scope requested; otherwise, REQUIRED.\",\n      \"pattern\": \"^[\\\\x21\\\\x23-\\\\x5B\\\\x5D-\\\\x7E]+(\\\\s[\\\\x21\\\\x23-\\\\x5B\\\\x5D-\\\\x7E]+)*$\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oauth/refs/heads/main/json-schema/oauth-token-response.json
tags:
- Access Control
- Authorization
- OAuth
- Security
- Tokens
title: OAuth 2.0 Token Response
---
