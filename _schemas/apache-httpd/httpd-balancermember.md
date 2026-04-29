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
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-httpd/json-schema/httpd-balancermember-schema.json\",\n  \"title\": \"BalancerMember\",\n  \"type\": \"object\",\n  \"description\": \"Member of a mod_proxy_balancer load balancing pool\",\n  \"properties\": {\n    \"url\": {\n      \"type\": \"string\",\n      \"description\": \"Backend URL\",\n      \"example\": \"http://backend1:8080\"\n    },\n    \"scheme\": {\n      \"type\": \"string\",\n      \"description\": \"Protocol scheme\",\n      \"example\": \"http\"\n    },\n    \"hostname\": {\n      \"type\": \"string\",\n      \"description\": \"Backend hostname\",\n      \"example\": \"backend1\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Backend port\",\n      \"example\": 8080\n    },\n    \"loadFactor\": {\n      \"type\": \"integer\",\n      \"description\": \"Load factor weight\",\n      \"example\": 1\n    },\n\
  \    \"lbStatus\": {\n      \"type\": \"string\",\n      \"description\": \"Load balancer member status\",\n      \"example\": \"Ok\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-httpd/refs/heads/main/json-schema/httpd-balancermember-schema.json
tags:
- Apache
- Load Balancer
- Open Source
- Proxy
- Reverse Proxy
- Web Server
title: BalancerMember
---
