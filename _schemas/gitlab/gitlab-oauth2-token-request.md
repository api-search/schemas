---
description: TokenRequest from GitLab API
layout: schema
name: TokenRequest
properties_list:
- description: The grant type for the token request.
  name: grant_type
  type: string
- description: The application ID registered in GitLab.
  name: client_id
  type: string
- description: The application secret. Required for confidential clients using authorization_code or refresh_token grant types.
  name: client_secret
  type: string
- description: The authorization code received from the authorize endpoint.
  name: code
  type: string
- description: The redirect URI used in the original authorization request.
  name: redirect_uri
  type: string
- description: The PKCE code verifier corresponding to the code_challenge.
  name: code_verifier
  type: string
- description: The refresh token to exchange for a new access token.
  name: refresh_token
  type: string
- description: The device code from the device authorization response.
  name: device_code
  type: string
- description: Resource owner username. Only for password grant type.
  name: username
  type: string
- description: Resource owner password. Only for password grant type.
  name: password
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-oauth2-token-request-schema.json
slug: gitlab-oauth2-token-request
source_filename: gitlab-oauth2-token-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-token-request-schema.json\",\n  \"title\": \"TokenRequest\",\n  \"description\": \"TokenRequest from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grant_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"authorization_code\",\n        \"refresh_token\",\n        \"device_code\",\n        \"password\"\n      ],\n      \"description\": \"The grant type for the token request.\",\n      \"example\": \"authorization_code\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The application ID registered in GitLab.\",\n      \"example\": \"123456\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"The application secret. Required for confidential clients using authorization_code or refresh_token\
  \ grant types.\",\n      \"example\": \"example_value\"\n    },\n    \"code\": {\n      \"type\": \"string\",\n      \"description\": \"The authorization code received from the authorize endpoint.\",\n      \"example\": \"example_value\"\n    },\n    \"redirect_uri\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The redirect URI used in the original authorization request.\",\n      \"example\": \"example_value\"\n    },\n    \"code_verifier\": {\n      \"type\": \"string\",\n      \"description\": \"The PKCE code verifier corresponding to the code_challenge.\",\n      \"example\": \"example_value\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"The refresh token to exchange for a new access token.\",\n      \"example\": \"main\"\n    },\n    \"device_code\": {\n      \"type\": \"string\",\n      \"description\": \"The device code from the device authorization response.\",\n      \"example\": \"example_value\"\
  \n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Resource owner username. Only for password grant type.\",\n      \"example\": \"Example Project\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Resource owner password. Only for password grant type.\",\n      \"example\": \"example_value\"\n    }\n  },\n  \"required\": [\n    \"grant_type\",\n    \"client_id\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-token-request-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: TokenRequest
---
