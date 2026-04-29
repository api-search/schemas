---
description: ''
layout: schema
name: ProxyConfig
properties_list:
- description: ''
  name: check_host_against_uptime_tests
  type: boolean
- description: ''
  name: disable_strip_slash
  type: boolean
- description: ''
  name: enable_load_balancing
  type: boolean
- description: ''
  name: listen_path
  type: string
- description: ''
  name: preserve_host_header
  type: boolean
- description: ''
  name: strip_listen_path
  type: boolean
- description: ''
  name: target_list
  type: array
- description: ''
  name: target_url
  type: string
- description: ''
  name: transport
  type: object
provider_name: Tyk
provider_slug: tyk
schema_file: json-schema/tyk-gateway-proxy-config-schema.json
slug: tyk-gateway-proxy-config
source_filename: tyk-gateway-proxy-config-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProxyConfig\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"check_host_against_uptime_tests\": {\n      \"type\": \"boolean\"\n    },\n    \"disable_strip_slash\": {\n      \"type\": \"boolean\"\n    },\n    \"enable_load_balancing\": {\n      \"type\": \"boolean\"\n    },\n    \"listen_path\": {\n      \"type\": \"string\"\n    },\n    \"preserve_host_header\": {\n      \"type\": \"boolean\"\n    },\n    \"strip_listen_path\": {\n      \"type\": \"boolean\"\n    },\n    \"target_list\": {\n      \"type\": \"array\"\n    },\n    \"target_url\": {\n      \"type\": \"string\"\n    },\n    \"transport\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/tyk/refs/heads/main/json-schema/tyk-gateway-proxy-config-schema.json
tags:
- API Gateway
- API Management
- GraphQL
- Open Source
title: ProxyConfig
---
