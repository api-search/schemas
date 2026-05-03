---
description: Schema describing the OpenID Provider Configuration Information document as defined in OpenID Connect Discovery 1.0. This document advertises the provider's capabilities, supported endpoints, signing algorithms, and other metadata that clients need to interact with the provider.
layout: schema
name: OpenID Connect Discovery Document
properties_list:
- description: The issuer identifier for the OpenID Provider. This value is used as the 'iss' claim in ID tokens and must be identical to the URL used to retrieve the discovery document.
  name: issuer
  type: string
- description: URL of the authorization endpoint where authentication requests are sent.
  name: authorization_endpoint
  type: string
- description: URL of the token endpoint used to exchange authorization codes for tokens.
  name: token_endpoint
  type: string
- description: URL of the UserInfo endpoint for retrieving claims about the authenticated user.
  name: userinfo_endpoint
  type: string
- description: URL of the JSON Web Key Set document containing the provider's public signing keys.
  name: jwks_uri
  type: string
- description: URL of the Dynamic Client Registration endpoint.
  name: registration_endpoint
  type: string
- description: List of OAuth 2.0 scope values supported by the provider.
  name: scopes_supported
  type: array
- description: List of OAuth 2.0 response_type values supported.
  name: response_types_supported
  type: array
- description: List of OAuth 2.0 response_mode values supported.
  name: response_modes_supported
  type: array
- description: List of OAuth 2.0 grant type values supported.
  name: grant_types_supported
  type: array
- description: List of Authentication Context Class Reference values supported.
  name: acr_values_supported
  type: array
- description: List of Subject Identifier types supported (public or pairwise).
  name: subject_types_supported
  type: array
- description: List of JWS signing algorithms supported for ID tokens.
  name: id_token_signing_alg_values_supported
  type: array
- description: List of JWE encryption algorithms (alg values) supported for ID tokens.
  name: id_token_encryption_alg_values_supported
  type: array
- description: List of JWE encryption algorithms (enc values) supported for ID tokens.
  name: id_token_encryption_enc_values_supported
  type: array
- description: List of JWS signing algorithms supported for UserInfo responses.
  name: userinfo_signing_alg_values_supported
  type: array
- description: List of JWE encryption algorithms supported for UserInfo responses.
  name: userinfo_encryption_alg_values_supported
  type: array
- description: List of JWS signing algorithms supported for Request Objects.
  name: request_object_signing_alg_values_supported
  type: array
- description: List of client authentication methods supported by the token endpoint.
  name: token_endpoint_auth_methods_supported
  type: array
- description: List of JWS signing algorithms supported for token endpoint authentication.
  name: token_endpoint_auth_signing_alg_values_supported
  type: array
- description: List of display parameter values supported.
  name: display_values_supported
  type: array
- description: List of Claim Types supported (normal, aggregated, distributed).
  name: claim_types_supported
  type: array
- description: List of Claim Names that the provider may supply values for.
  name: claims_supported
  type: array
- description: Whether the provider supports the 'claims' request parameter.
  name: claims_parameter_supported
  type: boolean
- description: Whether the provider supports the 'request' parameter for passing Request Objects.
  name: request_parameter_supported
  type: boolean
- description: Whether the provider supports the 'request_uri' parameter for passing Request Object by reference.
  name: request_uri_parameter_supported
  type: boolean
- description: Whether the provider requires request_uri values to be pre-registered.
  name: require_request_uri_registration
  type: boolean
- description: List of PKCE code challenge methods supported.
  name: code_challenge_methods_supported
  type: array
- description: URL of the end session endpoint for RP-Initiated Logout.
  name: end_session_endpoint
  type: string
- description: URL of the token introspection endpoint.
  name: introspection_endpoint
  type: string
- description: URL of the token revocation endpoint.
  name: revocation_endpoint
  type: string
- description: URL of a page with human-readable information about the provider.
  name: service_documentation
  type: string
- description: URL of the provider's policy document describing how client data is used.
  name: op_policy_uri
  type: string
- description: URL of the provider's terms of service document.
  name: op_tos_uri
  type: string
provider_name: OIDC
provider_slug: oidc
schema_file: json-schema/oidc-discovery.json
slug: oidc-discovery
source_filename: oidc-discovery.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"oidc-discovery.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenID Connect Discovery Document\",\n  \"description\": \"Schema describing the OpenID Provider Configuration Information document as defined in OpenID Connect Discovery 1.0. This document advertises the provider's capabilities, supported endpoints, signing algorithms, and other metadata that clients need to interact with the provider.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"issuer\",\n    \"authorization_endpoint\",\n    \"jwks_uri\",\n    \"response_types_supported\",\n    \"subject_types_supported\",\n    \"id_token_signing_alg_values_supported\"\n  ],\n  \"properties\": {\n    \"issuer\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The issuer identifier for the OpenID Provider. This value is used as the 'iss' claim in ID tokens and must be identical to the URL used to retrieve the discovery document.\"\
  \n    },\n    \"authorization_endpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the authorization endpoint where authentication requests are sent.\"\n    },\n    \"token_endpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the token endpoint used to exchange authorization codes for tokens.\"\n    },\n    \"userinfo_endpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the UserInfo endpoint for retrieving claims about the authenticated user.\"\n    },\n    \"jwks_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the JSON Web Key Set document containing the provider's public signing keys.\"\n    },\n    \"registration_endpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the Dynamic Client Registration endpoint.\"\n    },\n    \"scopes_supported\"\
  : {\n      \"type\": \"array\",\n      \"description\": \"List of OAuth 2.0 scope values supported by the provider.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"openid\", \"profile\", \"email\", \"address\", \"phone\", \"offline_access\"]\n      ]\n    },\n    \"response_types_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of OAuth 2.0 response_type values supported.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"code\", \"id_token\", \"id_token token\", \"code id_token\"]\n      ]\n    },\n    \"response_modes_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of OAuth 2.0 response_mode values supported.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"query\", \"fragment\", \"form_post\"]\n      ]\n    },\n    \"grant_types_supported\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"List of OAuth 2.0 grant type values supported.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"authorization_code\", \"implicit\", \"refresh_token\", \"client_credentials\"]\n      ]\n    },\n    \"acr_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of Authentication Context Class Reference values supported.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"subject_types_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of Subject Identifier types supported (public or pairwise).\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"public\", \"pairwise\"]\n      }\n    },\n    \"id_token_signing_alg_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of JWS signing algorithms supported for ID tokens.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"RS256\"\
  , \"RS384\", \"RS512\", \"ES256\", \"ES384\", \"ES512\", \"PS256\"]\n      ]\n    },\n    \"id_token_encryption_alg_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of JWE encryption algorithms (alg values) supported for ID tokens.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"id_token_encryption_enc_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of JWE encryption algorithms (enc values) supported for ID tokens.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"userinfo_signing_alg_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of JWS signing algorithms supported for UserInfo responses.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"userinfo_encryption_alg_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of JWE encryption algorithms supported for UserInfo responses.\",\n\
  \      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"request_object_signing_alg_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of JWS signing algorithms supported for Request Objects.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"token_endpoint_auth_methods_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of client authentication methods supported by the token endpoint.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"client_secret_basic\", \"client_secret_post\", \"client_secret_jwt\", \"private_key_jwt\", \"none\"]\n      ]\n    },\n    \"token_endpoint_auth_signing_alg_values_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of JWS signing algorithms supported for token endpoint authentication.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"display_values_supported\": {\n\
  \      \"type\": \"array\",\n      \"description\": \"List of display parameter values supported.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"page\", \"popup\", \"touch\", \"wap\"]\n      }\n    },\n    \"claim_types_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of Claim Types supported (normal, aggregated, distributed).\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"normal\", \"aggregated\", \"distributed\"]\n      }\n    },\n    \"claims_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of Claim Names that the provider may supply values for.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"examples\": [\n        [\"sub\", \"name\", \"given_name\", \"family_name\", \"email\", \"email_verified\", \"picture\", \"locale\"]\n      ]\n    },\n    \"claims_parameter_supported\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the provider\
  \ supports the 'claims' request parameter.\",\n      \"default\": false\n    },\n    \"request_parameter_supported\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the provider supports the 'request' parameter for passing Request Objects.\",\n      \"default\": false\n    },\n    \"request_uri_parameter_supported\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the provider supports the 'request_uri' parameter for passing Request Object by reference.\",\n      \"default\": true\n    },\n    \"require_request_uri_registration\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the provider requires request_uri values to be pre-registered.\",\n      \"default\": false\n    },\n    \"code_challenge_methods_supported\": {\n      \"type\": \"array\",\n      \"description\": \"List of PKCE code challenge methods supported.\",\n      \"items\": {\n        \"type\": \"string\",\n        \"enum\": [\"plain\", \"S256\"]\n      }\n    },\n\
  \    \"end_session_endpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the end session endpoint for RP-Initiated Logout.\"\n    },\n    \"introspection_endpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the token introspection endpoint.\"\n    },\n    \"revocation_endpoint\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the token revocation endpoint.\"\n    },\n    \"service_documentation\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of a page with human-readable information about the provider.\"\n    },\n    \"op_policy_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"URL of the provider's policy document describing how client data is used.\"\n    },\n    \"op_tos_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\"\
  : \"URL of the provider's terms of service document.\"\n    }\n  },\n  \"additionalProperties\": true\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/oidc/refs/heads/main/json-schema/oidc-discovery.json
tags:
- Authentication
- Identity
- JWT
- OAuth
- OIDC
- OpenID Connect
title: OpenID Connect Discovery Document
---
