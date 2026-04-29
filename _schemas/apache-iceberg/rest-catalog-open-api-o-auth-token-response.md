---
description: The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.
layout: schema
name: OAuthTokenResponse
properties_list:
- description: The access token, for client credentials or token exchange
  name: access_token
  type: string
- description: Access token type for client credentials or token exchange See https://datatracker.ietf.org/doc/html/rfc6749#section-7.1
  name: token_type
  type: string
- description: Lifetime of the access token in seconds for client credentials or token exchange
  name: expires_in
  type: integer
- description: ''
  name: issued_token_type
  type: object
- description: Refresh token for client credentials or token exchange
  name: refresh_token
  type: string
- description: Authorization scope for client credentials or token exchange
  name: scope
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-o-auth-token-response-schema.json
slug: rest-catalog-open-api-o-auth-token-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-token-response-schema.json\",\n  \"title\": \"OAuthTokenResponse\",\n  \"description\": \"The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"access_token\": {\n      \"type\": \"string\",\n      \"description\": \"The access token, for client credentials or token exchange\"\n    },\n    \"token_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"bearer\",\n        \"mac\",\n        \"N_A\"\n      ],\n      \"description\": \"Access token type for client credentials or token exchange\\n\\nSee https://datatracker.ietf.org/doc/html/rfc6749#section-7.1\"\n    },\n    \"expires_in\": {\n      \"type\": \"integer\",\n      \"description\"\
  : \"Lifetime of the access token in seconds for client credentials or token exchange\"\n    },\n    \"issued_token_type\": {\n      \"$ref\": \"#/components/schemas/TokenType\"\n    },\n    \"refresh_token\": {\n      \"type\": \"string\",\n      \"description\": \"Refresh token for client credentials or token exchange\"\n    },\n    \"scope\": {\n      \"type\": \"string\",\n      \"description\": \"Authorization scope for client credentials or token exchange\"\n    }\n  },\n  \"required\": [\n    \"access_token\",\n    \"token_type\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-token-response-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: OAuthTokenResponse
---
