---
description: An OAuth 2.0 token response from the ForgeRock Access Management token endpoint. Conforms to RFC 6749 and OpenID Connect Core specifications.
layout: schema
name: ForgeRock OAuth 2.0 Token Response
properties_list:
- description: The access token issued by the authorization server
  name: access_token
  type: string
- description: The type of token issued (typically Bearer)
  name: token_type
  type: string
- description: Lifetime of the access token in seconds
  name: expires_in
  type: integer
- description: Refresh token that can be used to obtain new access tokens
  name: refresh_token
  type: string
- description: Space-delimited list of scopes granted to the access token
  name: scope
  type: string
- description: OpenID Connect ID token (JWT) when openid scope is requested
  name: id_token
  type: string
provider_name: ForgeRock
provider_slug: forgerock
schema_file: json-schema/forgerock-oauth2-token-schema.json
slug: forgerock-oauth2-token
source_filename: forgerock-oauth2-token-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://schema.forgerock.com/oauth2-token\",\n  \"title\": \"ForgeRock OAuth 2.0 Token Response\",\n  \"description\": \"An OAuth 2.0 token response from the ForgeRock Access Management token endpoint. Conforms to RFC 6749 and OpenID Connect Core specifications.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"The access token issued by the authorization server\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of token issued (typically Bearer)\",\n      \"enum\": [\"Bearer\"]\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Lifetime of the access token in seconds\",\n      \"minimum\": 0\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"Refresh token that can be used to obtain new access tokens\"\
  \n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Space-delimited list of scopes granted to the access token\"\n    },\n    \"id_token\": {\n      \"type\": \"string\",\n      \"description\": \"OpenID Connect ID token (JWT) when openid scope is requested\"\n    }\n  },\n  \"required\": [\"access_token\", \"token_type\", \"expires_in\"]\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/json-schema/forgerock-oauth2-token-schema.json
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
title: ForgeRock OAuth 2.0 Token Response
---
