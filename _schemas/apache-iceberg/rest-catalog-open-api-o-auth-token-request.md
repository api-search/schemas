---
description: The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.
layout: schema
name: OAuthTokenRequest
properties_list: []
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-o-auth-token-request-schema.json
slug: rest-catalog-open-api-o-auth-token-request
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-token-request-schema.json\",\n  \"title\": \"OAuthTokenRequest\",\n  \"description\": \"The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.\",\n  \"anyOf\": [\n    {\n      \"$ref\": \"#/components/schemas/OAuthClientCredentialsRequest\"\n    },\n    {\n      \"$ref\": \"#/components/schemas/OAuthTokenExchangeRequest\"\n    }\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-token-request-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: OAuthTokenRequest
---
