---
description: Configuration details for a supported OAuth Flow.
layout: schema
name: OpenAPI OAuth Flow Object
properties_list:
- description: The authorization URL for this flow.
  name: authorizationUrl
  type: string
- description: The token URL for this flow.
  name: tokenUrl
  type: string
- description: The URL to be used for obtaining refresh tokens.
  name: refreshUrl
  type: string
- description: The available scopes for the OAuth2 security scheme.
  name: scopes
  type: object
provider_name: OpenAPI
provider_slug: openapi
schema_file: json-schema/openapi-oauth-flow.json
slug: openapi-oauth-flow
source_filename: openapi-oauth-flow.json
source_heading: JSON Schema
source_json: "{\n  \"$id\": \"openapi-oauth-flow.json\",\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"OpenAPI OAuth Flow Object\",\n  \"description\": \"Configuration details for a supported OAuth Flow.\",\n  \"type\": \"object\",\n  \"required\": [\n    \"scopes\"\n  ],\n  \"properties\": {\n    \"authorizationUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The authorization URL for this flow.\"\n    },\n    \"tokenUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The token URL for this flow.\"\n    },\n    \"refreshUrl\": {\n      \"type\": \"string\",\n      \"format\": \"uri\",\n      \"description\": \"The URL to be used for obtaining refresh tokens.\"\n    },\n    \"scopes\": {\n      \"type\": \"object\",\n      \"description\": \"The available scopes for the OAuth2 security scheme.\",\n      \"additionalProperties\": {\n        \"type\": \"string\"\n      }\n\
  \    }\n  },\n  \"patternProperties\": {\n    \"^x-\": {}\n  },\n  \"additionalProperties\": false\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/openapi/refs/heads/main/json-schema/openapi-oauth-flow.json
tags:
- Documentation
- REST
- Specification
title: OpenAPI OAuth Flow Object
---
