---
description: TokenInfo from GitLab API
layout: schema
name: TokenInfo
properties_list:
- description: The ID of the user who authorized the token.
  name: resource_owner_id
  type: integer
- description: Information about the OAuth application.
  name: application
  type: object
- description: List of scopes the token has been granted.
  name: scope
  type: array
- description: Remaining lifetime of the token in seconds.
  name: expires_in_seconds
  type: integer
- description: Unix timestamp of when the token was created.
  name: created_at
  type: number
provider_name: GitLab
provider_slug: gitlab
schema_file: json-schema/gitlab-oauth2-token-info-schema.json
slug: gitlab-oauth2-token-info
source_filename: gitlab-oauth2-token-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-token-info-schema.json\",\n  \"title\": \"TokenInfo\",\n  \"description\": \"TokenInfo from GitLab API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"resource_owner_id\": {\n      \"type\": \"integer\",\n      \"description\": \"The ID of the user who authorized the token.\",\n      \"example\": 42\n    },\n    \"application\": {\n      \"type\": \"object\",\n      \"description\": \"Information about the OAuth application.\",\n      \"properties\": {\n        \"uid\": {\n          \"type\": \"string\",\n          \"description\": \"The application client ID.\"\n        }\n      }\n    },\n    \"scope\": {\n      \"type\": \"array\",\n      \"description\": \"List of scopes the token has been granted.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"expires_in_seconds\"\
  : {\n      \"type\": \"integer\",\n      \"description\": \"Remaining lifetime of the token in seconds.\",\n      \"example\": 42\n    },\n    \"created_at\": {\n      \"type\": \"number\",\n      \"description\": \"Unix timestamp of when the token was created.\",\n      \"example\": 42.5\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/gitlab/refs/heads/main/json-schema/gitlab-oauth2-token-info-schema.json
tags:
- Code
- Platform
- Software Development
- Source Control
title: TokenInfo
---
