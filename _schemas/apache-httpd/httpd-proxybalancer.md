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
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-httpd/json-schema/httpd-proxybalancer-schema.json\",\n  \"title\": \"ProxyBalancer\",\n  \"type\": \"object\",\n  \"description\": \"Apache mod_proxy_balancer pool configuration and status\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Balancer URL\",\n      \"example\": \"balancer://mycluster\"\n    },\n    \"lbMethod\": {\n      \"type\": \"string\",\n      \"description\": \"Load balancing method\",\n      \"example\": \"byrequests\"\n    },\n    \"nonce\": {\n      \"type\": \"string\",\n      \"description\": \"Security nonce for balancer-manager\",\n      \"example\": \"abc123\"\n    },\n    \"members\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"$ref\": \"#/components/schemas/BalancerMember\"\n      },\n      \"description\": \"Balancer member backends\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-httpd/refs/heads/main/json-schema/httpd-proxybalancer-schema.json
tags:
- Apache
- Load Balancer
- Open Source
- Proxy
- Reverse Proxy
- Web Server
title: ProxyBalancer
---
