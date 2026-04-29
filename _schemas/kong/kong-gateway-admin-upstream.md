---
description: An Upstream object represents a virtual hostname and can be used to health-check, circuit-break, and load-balance incoming requests over multiple services.
layout: schema
name: Upstream
properties_list:
- description: ''
  name: id
  type: string
- description: A hostname which must be equal to the host of a Service.
  name: name
  type: string
- description: The load balancing algorithm to use.
  name: algorithm
  type: string
- description: What to use as hashing input when the consistent-hashing algorithm is selected.
  name: hash_on
  type: string
- description: What to use as hashing input if the primary hash_on does not return a hash.
  name: hash_fallback
  type: string
- description: The header name to take the value from as hash input (when hash_on is set to header).
  name: hash_on_header
  type: string
- description: ''
  name: hash_fallback_header
  type: string
- description: ''
  name: hash_on_cookie
  type: string
- description: ''
  name: hash_on_cookie_path
  type: string
- description: ''
  name: hash_on_query_arg
  type: string
- description: ''
  name: hash_fallback_query_arg
  type: string
- description: ''
  name: hash_on_uri_capture
  type: string
- description: ''
  name: hash_fallback_uri_capture
  type: string
- description: The number of slots in the load balancer algorithm.
  name: slots
  type: integer
- description: ''
  name: tags
  type: array
- description: The hostname to be used as Host header when proxying requests through ring-balancer.
  name: host_header
  type: string
- description: If set, balancer will use SRV hostname as the proxy Host header.
  name: use_srv_name
  type: boolean
- description: ''
  name: created_at
  type: integer
- description: ''
  name: updated_at
  type: integer
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-upstream-schema.json
slug: kong-gateway-admin-upstream
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Upstream\",\n  \"type\": \"object\",\n  \"description\": \"An Upstream object represents a virtual hostname and can be used to health-check, circuit-break, and load-balance incoming requests over multiple services.\",\n  \"properties\": {\n    \"id\": {\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"A hostname which must be equal to the host of a Service.\"\n    },\n    \"algorithm\": {\n      \"type\": \"string\",\n      \"description\": \"The load balancing algorithm to use.\"\n    },\n    \"hash_on\": {\n      \"type\": \"string\",\n      \"description\": \"What to use as hashing input when the consistent-hashing algorithm is selected.\"\n    },\n    \"hash_fallback\": {\n      \"type\": \"string\",\n      \"description\": \"What to use as hashing input if the primary hash_on does not return a hash.\"\n    },\n    \"hash_on_header\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The header name to take the value from as hash input (when hash_on is set to header).\"\n    },\n    \"hash_fallback_header\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_cookie\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_cookie_path\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_query_arg\": {\n      \"type\": \"string\"\n    },\n    \"hash_fallback_query_arg\": {\n      \"type\": \"string\"\n    },\n    \"hash_on_uri_capture\": {\n      \"type\": \"string\"\n    },\n    \"hash_fallback_uri_capture\": {\n      \"type\": \"string\"\n    },\n    \"slots\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of slots in the load balancer algorithm.\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"host_header\": {\n      \"type\": \"string\",\n      \"description\": \"The hostname to be used as Host header when proxying requests through ring-balancer.\"\n    },\n \
  \   \"use_srv_name\": {\n      \"type\": \"boolean\",\n      \"description\": \"If set, balancer will use SRV hostname as the proxy Host header.\"\n    },\n    \"created_at\": {\n      \"type\": \"integer\"\n    },\n    \"updated_at\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-upstream-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: Upstream
---
