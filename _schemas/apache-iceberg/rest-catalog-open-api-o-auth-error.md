---
description: The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.
layout: schema
name: OAuthError
properties_list:
- description: ''
  name: error
  type: string
- description: ''
  name: error_description
  type: string
- description: ''
  name: error_uri
  type: string
provider_name: Apache Iceberg
provider_slug: apache-iceberg
schema_file: json-schema/rest-catalog-open-api-o-auth-error-schema.json
slug: rest-catalog-open-api-o-auth-error
source_filename: rest-catalog-open-api-o-auth-error-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-error-schema.json\",\n  \"title\": \"OAuthError\",\n  \"description\": \"The `oauth/tokens` endpoint and related schemas are **DEPRECATED for REMOVAL** from this spec, see description of the endpoint.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"error\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"invalid_request\",\n        \"invalid_client\",\n        \"invalid_grant\",\n        \"unauthorized_client\",\n        \"unsupported_grant_type\",\n        \"invalid_scope\"\n      ]\n    },\n    \"error_description\": {\n      \"type\": \"string\"\n    },\n    \"error_uri\": {\n      \"type\": \"string\"\n    }\n  },\n  \"required\": [\n    \"error\"\n  ],\n  \"deprecated\": true\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-iceberg/refs/heads/main/json-schema/rest-catalog-open-api-o-auth-error-schema.json
tags:
- ACID
- Analytics
- Apache
- Data Lake
- Lakehouse
- Open Source
- Table Format
title: OAuthError
---
