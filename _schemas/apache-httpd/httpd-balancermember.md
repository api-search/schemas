---
description: Member of a mod_proxy_balancer load balancing pool
layout: schema
name: BalancerMember
properties_list:
- description: Backend URL
  name: url
  type: string
- description: Protocol scheme
  name: scheme
  type: string
- description: Backend hostname
  name: hostname
  type: string
- description: Backend port
  name: port
  type: integer
- description: Load factor weight
  name: loadFactor
  type: integer
- description: Load balancer member status
  name: lbStatus
  type: string
provider_name: Apache HTTP Server
provider_slug: apache-httpd
schema_file: json-schema/httpd-balancermember-schema.json
slug: httpd-balancermember
tags:
- Apache
- Load Balancer
- Open Source
- Proxy
- Reverse Proxy
- Web Server
title: BalancerMember
---
