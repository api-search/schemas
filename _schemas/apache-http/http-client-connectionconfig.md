---
description: Connection configuration for Apache HttpComponents client
layout: schema
name: ConnectionConfig
properties_list:
- description: Connection timeout in milliseconds
  name: connectTimeout
  type: integer
- description: Socket read timeout in milliseconds
  name: socketTimeout
  type: integer
- description: Maximum total connections in pool
  name: maxConnections
  type: integer
- description: Maximum connections per route
  name: maxConnectionsPerRoute
  type: integer
- description: Keep-alive timeout in milliseconds
  name: keepAliveTimeout
  type: integer
provider_name: Apache HttpComponents
provider_slug: apache-http
schema_file: json-schema/http-client-connectionconfig-schema.json
slug: http-client-connectionconfig
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-http/json-schema/http-client-connectionconfig-schema.json\",\n  \"title\": \"ConnectionConfig\",\n  \"type\": \"object\",\n  \"description\": \"Connection configuration for Apache HttpComponents client\",\n  \"properties\": {\n    \"connectTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Connection timeout in milliseconds\",\n      \"example\": 5000\n    },\n    \"socketTimeout\": {\n      \"type\": \"integer\",\n      \"description\": \"Socket read timeout in milliseconds\",\n      \"example\": 30000\n    },\n    \"maxConnections\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum total connections in pool\",\n      \"example\": 200\n    },\n    \"maxConnectionsPerRoute\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum connections per route\",\n      \"example\": 20\n    },\n    \"keepAliveTimeout\": {\n\
  \      \"type\": \"integer\",\n      \"description\": \"Keep-alive timeout in milliseconds\",\n      \"example\": 60000\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-http/refs/heads/main/json-schema/http-client-connectionconfig-schema.json
tags:
- Apache
- HTTP Client
- Java
- Open Source
- SDK
title: ConnectionConfig
---
