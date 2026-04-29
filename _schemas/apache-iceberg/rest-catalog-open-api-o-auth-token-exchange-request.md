---
description: The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint. OAuth2 token exchange request See https://datatracker.ietf.org/doc/html/rfc8693
layout: schema
name: OAuthTokenExchangeRequest
properties_list:
- description: ''
  name: grant_type
  type: string
- description: ''
  name: scope
  type: string
- description: ''
  name: requested_token_type
  type: object
- description: Subject token for token exchange request
  name: subject_token
  type: string
- description: ''
  name: subject_token_type
  type: object
- description: Actor token for token exchange request
  name: actor_token
  type: string
- description: ''
  name: actor_token_type
  type: object
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-o-auth-token-exchange-request-schema.json
slug: rest-catalog-open-api-o-auth-token-exchange-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-token-exchange-request-schema.json\",\n  \"title\": \"OAuthTokenExchangeRequest\",\n  \"description\": \"The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.\\n\\nOAuth2 token exchange request\\n\\nSee https://datatracker.ietf.org/doc/html/rfc8693\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grant_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"urn:ietf:params:oauth:grant-type:token-exchange\"\n      ]\n    },\n    \"scope\": {\n      \"type\": \"string\"\n    },\n    \"requested_token_type\": {\n      \"$ref\": \"#/components/schemas/TokenType\"\n    },\n    \"subject_token\": {\n      \"type\": \"string\",\n      \"description\": \"Subject token for token exchange request\"\
  \n    },\n    \"subject_token_type\": {\n      \"$ref\": \"#/components/schemas/TokenType\"\n    },\n    \"actor_token\": {\n      \"type\": \"string\",\n      \"description\": \"Actor token for token exchange request\"\n    },\n    \"actor_token_type\": {\n      \"$ref\": \"#/components/schemas/TokenType\"\n    }\n  },\n  \"required\": [\n    \"grant_type\",\n    \"subject_token\",\n    \"subject_token_type\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-token-exchange-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: OAuthTokenExchangeRequest
---
