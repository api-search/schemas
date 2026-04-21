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
tags:
- Apache
- HTTP Client
- Java
- Open Source
- SDK
title: ConnectionConfig
---
