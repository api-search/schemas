---
description: Schema describing the parameters of an OAuth 2.0 authorization request as defined in RFC 6749 Section 4.1.1 (Authorization Code Grant) and Section 4.2.1 (Implicit Grant). These parameters are sent as query components of the authorization endpoint URI.
layout: schema
name: OAuth 2.0 Authorization Request
properties_list:
- description: The value MUST be 'code' for requesting an authorization code (Section 4.1.1) or 'token' for requesting an access token via the implicit grant (Section 4.2.1).
  name: response_type
  type: string
- description: The client identifier as described in RFC 6749 Section 2.2.
  name: client_id
  type: string
- description: The absolute URI to which the authorization server will redirect the user-agent after authorization. As described in Section 3.1.2.
  name: redirect_uri
  type: string
- description: The scope of the access request as a space-delimited list of case-sensitive scope values. As described in Section 3.3.
  name: scope
  type: string
- description: An opaque value used by the client to maintain state between the request and callback. The authorization server includes this value when redirecting back to the client. SHOULD be used to prevent cross
  name: state
  type: string
- description: PKCE code challenge derived from the code verifier, as defined in RFC 7636 Section 4.2.
  name: code_challenge
  type: string
- description: PKCE code challenge method. Defaults to 'plain' if not present. As defined in RFC 7636 Section 4.3.
  name: code_challenge_method
  type: string
provider_name: OAuth
provider_slug: oauth
schema_file: json-schema/oauth-authorization-request.json
slug: oauth-authorization-request
source_filename: oauth-authorization-request.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"oauth-authorization-request.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OAuth 2.0 Authorization Request\",\n  \"description\": \"Schema describing the parameters of an OAuth 2.0 authorization request as defined in RFC 6749 Section 4.1.1 (Authorization Code Grant) and Section 4.2.1 (Implicit Grant). These parameters are sent as query components of the authorization endpoint URI.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"response_type\",\n    \"client_id\"\n  ],\n  \"properties\": {\n    \"response_type\": {\n      \"type\": \"string\",\n      \"description\": \"The value MUST be 'code' for requesting an authorization code (Section 4.1.1) or 'token' for requesting an access token via the implicit grant (Section 4.2.1).\",\n      \"enum\": [\n        \"code\",\n        \"token\"\n      ]\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The client identifier as described\
  \ in RFC 6749 Section 2.2.\"\n    },\n    \"redirect_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The absolute URI to which the authorization server will redirect the user-agent after authorization. As described in Section 3.1.2.\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"The scope of the access request as a space-delimited list of case-sensitive scope values. As described in Section 3.3.\",\n      \"pattern\": \"^[\\\\x21\\\\x23-\\\\x5B\\\\x5D-\\\\x7E]+(\\\\s[\\\\x21\\\\x23-\\\\x5B\\\\x5D-\\\\x7E]+)*$\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"An opaque value used by the client to maintain state between the request and callback. The authorization server includes this value when redirecting back to the client. SHOULD be used to prevent cross-site request forgery (CSRF) attacks.\"\n    },\n    \"code_challenge\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"PKCE code challenge derived from the code verifier, as defined in RFC 7636 Section 4.2.\",\n      \"minLength\": 43,\n      \"maxLength\": 128\n    },\n    \"code_challenge_method\": {\n      \"type\": \"string\",\n      \"description\": \"PKCE code challenge method. Defaults to 'plain' if not present. As defined in RFC 7636 Section 4.3.\",\n      \"enum\": [\n        \"plain\",\n        \"S256\"\n      ],\n      \"default\": \"plain\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oauth/refs/heads/main/json-schema/oauth-authorization-request.json
tags:
- Access Control
- Authorization
- OAuth
- Security
- Tokens
title: OAuth 2.0 Authorization Request
---
