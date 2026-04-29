---
description: The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint. OAuth2 client credentials request See https://datatracker.ietf.org/doc/html/rfc6749#section-4.4
layout: schema
name: OAuthClientCredentialsRequest
properties_list:
- description: ''
  name: grant_type
  type: string
- description: ''
  name: scope
  type: string
- description: Client ID This can be sent in the request body, but OAuth2 recommends sending it in a Basic Authorization header.
  name: client_id
  type: string
- description: Client secret This can be sent in the request body, but OAuth2 recommends sending it in a Basic Authorization header.
  name: client_secret
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-o-auth-client-credentials-request-schema.json
slug: rest-catalog-open-api-o-auth-client-credentials-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-client-credentials-request-schema.json\",\n  \"title\": \"OAuthClientCredentialsRequest\",\n  \"description\": \"The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.\\n\\nOAuth2 client credentials request\\n\\nSee https://datatracker.ietf.org/doc/html/rfc6749#section-4.4\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"grant_type\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"client_credentials\"\n      ]\n    },\n    \"scope\": {\n      \"type\": \"string\"\n    },\n    \"client_id\": {\n      \"type\": \"string\",\n      \"description\": \"Client ID\\n\\nThis can be sent in the request body, but OAuth2 recommends sending it in a Basic Authorization header.\"\n    },\n    \"client_secret\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"Client secret\\n\\nThis can be sent in the request body, but OAuth2 recommends sending it in a Basic Authorization header.\"\n    }\n  },\n  \"required\": [\n    \"grant_type\",\n    \"client_id\",\n    \"client_secret\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-client-credentials-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: OAuthClientCredentialsRequest
---
