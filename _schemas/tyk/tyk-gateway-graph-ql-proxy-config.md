---
description: ''
layout: schema
name: GraphQLProxyConfig
properties_list:
- description: ''
  name: auth_headers
  type: object
- description: ''
  name: request_headers
  type: object
- description: ''
  name: request_headers_rewrite
  type: object
- description: ''
  name: subscription_type
  type: string
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-graph-ql-proxy-config-schema.json
slug: tyk-gateway-graph-ql-proxy-config
source_filename: tyk-gateway-graph-ql-proxy-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GraphQLProxyConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"auth_headers\": {\n      \"type\": \"object\"\n    },\n    \"request_headers\": {\n      \"type\": \"object\"\n    },\n    \"request_headers_rewrite\": {\n      \"type\": \"object\"\n    },\n    \"subscription_type\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-graph-ql-proxy-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: GraphQLProxyConfig
---
