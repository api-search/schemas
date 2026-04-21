---
description: HTTP proxy configuration for Apache HttpComponents client
layout: schema
name: ProxyConfig
properties_list:
- description: Proxy hostname
  name: host
  type: string
- description: Proxy port
  name: port
  type: integer
- description: Proxy scheme (http or https)
  name: scheme
  type: string
- description: Proxy authentication username
  name: username
  type: string
- description: Proxy authentication password
  name: password
  type: string
provider_name: Apache HttpComponents
provider_slug: apache-http
schema_file: json-schema/http-client-proxyconfig-schema.json
slug: http-client-proxyconfig
tags:
- Apache
- HTTP Client
- Java
- Open Source
- SDK
title: ProxyConfig
---
