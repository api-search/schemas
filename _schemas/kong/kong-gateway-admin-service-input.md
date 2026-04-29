---
description: Input schema for creating or updating a Service.
layout: schema
name: ServiceInput
properties_list:
- description: An optional human-readable name for the Service.
  name: name
  type: string
- description: ''
  name: protocol
  type: string
- description: The host of the upstream server.
  name: host
  type: string
- description: ''
  name: port
  type: integer
- description: ''
  name: path
  type: string
- description: ''
  name: retries
  type: integer
- description: ''
  name: connect_timeout
  type: integer
- description: ''
  name: write_timeout
  type: integer
- description: ''
  name: read_timeout
  type: integer
- description: Shorthand attribute to set protocol, host, port, and path at once.
  name: url
  type: string
- description: ''
  name: tags
  type: array
- description: ''
  name: client_certificate
  type: object
- description: ''
  name: tls_verify
  type: boolean
- description: ''
  name: tls_verify_depth
  type: integer
- description: ''
  name: ca_certificates
  type: array
- description: ''
  name: enabled
  type: boolean
provider_name: Kong
provider_slug: kong
schema_file: json-schema/kong-gateway-admin-service-input-schema.json
slug: kong-gateway-admin-service-input
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ServiceInput\",\n  \"type\": \"object\",\n  \"description\": \"Input schema for creating or updating a Service.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"An optional human-readable name for the Service.\"\n    },\n    \"protocol\": {\n      \"type\": \"string\"\n    },\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"The host of the upstream server.\"\n    },\n    \"port\": {\n      \"type\": \"integer\"\n    },\n    \"path\": {\n      \"type\": \"string\"\n    },\n    \"retries\": {\n      \"type\": \"integer\"\n    },\n    \"connect_timeout\": {\n      \"type\": \"integer\"\n    },\n    \"write_timeout\": {\n      \"type\": \"integer\"\n    },\n    \"read_timeout\": {\n      \"type\": \"integer\"\n    },\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Shorthand attribute to set protocol, host,\
  \ port, and path at once.\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\n    },\n    \"client_certificate\": {\n      \"type\": \"object\"\n    },\n    \"tls_verify\": {\n      \"type\": \"boolean\"\n    },\n    \"tls_verify_depth\": {\n      \"type\": \"integer\"\n    },\n    \"ca_certificates\": {\n      \"type\": \"array\"\n    },\n    \"enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/json-schema/kong-gateway-admin-service-input-schema.json
tags:
- API Gateway
- Lua
- NGINX
- Open Source
title: ServiceInput
---
