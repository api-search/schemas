---
description: Apache mod_proxy_balancer pool configuration and status
layout: schema
name: ProxyBalancer
properties_list:
- description: Balancer URL
  name: url
  type: string
- description: Load balancing method
  name: lbMethod
  type: string
- description: Security nonce for balancer-manager
  name: nonce
  type: string
- description: Balancer member backends
  name: members
  type: array
provider_name: Apache HTTP Server
provider_slug: apache-httpd
schema_file: json-schema/httpd-proxybalancer-schema.json
slug: httpd-proxybalancer
tags:
- Apache
- Load Balancer
- Open Source
- Proxy
- Reverse Proxy
- Web Server
title: ProxyBalancer
---
