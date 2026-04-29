---
description: InitiateOauthRequest schema from Airbyte API
layout: schema
name: InitiateOauthRequest
properties_list:
- description: The name of the source to authenticate to. Deprecated - use sourceType instead.
  name: name
  type: string
- description: The name of the source to authenticate to
  name: sourceType
  type: string
- description: The URL to redirect the user to with the OAuth secret stored in the secret_id query string parameter after authentication is complete.
  name: redirectUrl
  type: string
- description: The workspace to create the secret and eventually the full source.
  name: workspaceId
  type: string
- description: Input configuration for OAuth required by some sources.
  name: oAuthInputConfiguration
  type: object
- description: Optional OAuth scopes to request, overriding the connector's default scopes. Only supported for connectors that define scopes as an array.
  name: requestedScopes
  type: array
- description: Optional OAuth optional_scopes to request, overriding the connector's default optional_scopes. Only applied when requestedScopes is also provided.
  name: requestedOptionalScopes
  type: array
provider_name: Airbyte
provider_slug: airbyte
schema_file: json-schema/airbyte-initiate-oauth-request-schema.json
slug: airbyte-initiate-oauth-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-initiate-oauth-request-schema.json\",\n  \"title\": \"InitiateOauthRequest\",\n  \"description\": \"InitiateOauthRequest schema from Airbyte API\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"name\": {\n      \"description\": \"The name of the source to authenticate to. Deprecated - use sourceType instead.\",\n      \"type\": \"string\"\n    },\n    \"sourceType\": {\n      \"description\": \"The name of the source to authenticate to\",\n      \"type\": \"string\"\n    },\n    \"redirectUrl\": {\n      \"description\": \"The URL to redirect the user to with the OAuth secret stored in the secret_id query string parameter after authentication is complete.\",\n      \"type\": \"string\"\n    },\n    \"workspaceId\": {\n      \"format\": \"uuid\",\n      \"description\": \"The workspace to create\
  \ the secret and eventually the full source.\",\n      \"type\": \"string\"\n    },\n    \"oAuthInputConfiguration\": {\n      \"$ref\": \"#/components/schemas/OAuthInputConfiguration\",\n      \"description\": \"Input configuration for OAuth required by some sources.\"\n    },\n    \"requestedScopes\": {\n      \"type\": \"array\",\n      \"description\": \"Optional OAuth scopes to request, overriding the connector's default scopes. Only supported for connectors that define scopes as an array.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    },\n    \"requestedOptionalScopes\": {\n      \"type\": \"array\",\n      \"description\": \"Optional OAuth optional_scopes to request, overriding the connector's default optional_scopes. Only applied when requestedScopes is also provided.\",\n      \"items\": {\n        \"type\": \"string\"\n      }\n    }\n  },\n  \"required\": [\n    \"redirectUrl\",\n    \"workspaceId\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/airbyte/refs/heads/main/json-schema/airbyte-initiate-oauth-request-schema.json
tags:
- Data Integration
- ETL
- ELT
- Open Source
- Data Pipeline
- Connectors
- Data
title: InitiateOauthRequest
---
