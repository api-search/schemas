---
description: TokenResponse from GitLab API
layout: schema
name: TokenResponse
properties_list:
- description: The OAuth 2.0 access token.
  name: access_token
  type: string
- description: The type of token. Always Bearer.
  name: token_type
  type: string
- description: Token lifetime in seconds. Typically 7200 (2 hours).
  name: expires_in
  type: integer
- description: The refresh token for obtaining new access tokens.
  name: refresh_token
  type: string
- description: Space-separated list of granted scopes.
  name: scope
  type: string
- description: Unix timestamp of when the token was created.
  name: created_at
  type: integer
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-oauth2-token-response-schema.json
slug: gitlab-oauth2-token-response
source_filename: gitlab-oauth2-token-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-token-response-schema.json\",\n  \"title\": \"TokenResponse\",\n  \"description\": \"TokenResponse from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"The OAuth 2.0 access token.\",\n      \"example\": \"glpat-example-token\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"description\": \"The type of token. Always Bearer.\",\n      \"example\": \"glpat-example-token\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\": \"Token lifetime in seconds. Typically 7200 (2 hours).\",\n      \"example\": 42\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"The refresh token for obtaining new access tokens.\",\n      \"example\"\
  : \"main\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Space-separated list of granted scopes.\",\n      \"example\": \"example_value\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\",\n      \"description\": \"Unix timestamp of when the token was created.\",\n      \"example\": 42\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-token-response-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: TokenResponse
---
