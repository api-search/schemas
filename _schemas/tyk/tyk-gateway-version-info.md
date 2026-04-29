---
description: ''
layout: schema
name: VersionInfo
properties_list:
- description: ''
  name: expires
  type: string
- description: ''
  name: global_headers
  type: object
- description: ''
  name: global_headers_disabled
  type: boolean
- description: ''
  name: global_headers_remove
  type: array
- description: ''
  name: global_response_headers
  type: object
- description: ''
  name: global_response_headers_disabled
  type: boolean
- description: ''
  name: global_response_headers_remove
  type: array
- description: ''
  name: global_size_limit
  type: integer
- description: ''
  name: ignore_endpoint_case
  type: boolean
- description: ''
  name: name
  type: string
- description: ''
  name: override_target
  type: string
- description: ''
  name: paths
  type: object
- description: ''
  name: use_extended_paths
  type: boolean
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-version-info-schema.json
slug: tyk-gateway-version-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VersionInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"expires\": {\n      \"type\": \"string\"\n    },\n    \"global_headers\": {\n      \"type\": \"object\"\n    },\n    \"global_headers_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"global_headers_remove\": {\n      \"type\": \"array\"\n    },\n    \"global_response_headers\": {\n      \"type\": \"object\"\n    },\n    \"global_response_headers_disabled\": {\n      \"type\": \"boolean\"\n    },\n    \"global_response_headers_remove\": {\n      \"type\": \"array\"\n    },\n    \"global_size_limit\": {\n      \"type\": \"integer\"\n    },\n    \"ignore_endpoint_case\": {\n      \"type\": \"boolean\"\n    },\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"override_target\": {\n      \"type\": \"string\"\n    },\n    \"paths\": {\n      \"type\": \"object\"\n    },\n    \"use_extended_paths\": {\n      \"type\"\
  : \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-version-info-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: VersionInfo
---
