---
description: RevokeTokenRequest from GitLab API
layout: schema
name: RevokeTokenRequest
properties_list:
- description: The application ID registered in GitLab.
  name: client_id
  type: string
- description: The application secret.
  name: client_secret
  type: string
- description: The access token or refresh token to revoke.
  name: token
  type: string
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-oauth2-revoke-token-request-schema.json
slug: gitlab-oauth2-revoke-token-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-revoke-token-request-schema.json\",\n  \"title\": \"RevokeTokenRequest\",\n  \"description\": \"RevokeTokenRequest from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"The application ID registered in GitLab.\",\n      \"example\": \"123456\"\n    },\n    \"client_secret\": {\n      \"type\": \"string\",\n      \"description\": \"The application secret.\",\n      \"example\": \"example_value\"\n    },\n    \"token\": {\n      \"type\": \"string\",\n      \"description\": \"The access token or refresh token to revoke.\",\n      \"example\": \"glpat-example-token\"\n    }\n  },\n  \"required\": [\n    \"client_id\",\n    \"client_secret\",\n    \"token\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-revoke-token-request-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: RevokeTokenRequest
---
