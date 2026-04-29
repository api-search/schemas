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
source_filename: http-client-proxyconfig-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-http/json-schema/http-client-proxyconfig-schema.json\",\n  \"title\": \"ProxyConfig\",\n  \"type\": \"object\",\n  \"description\": \"HTTP proxy configuration for Apache HttpComponents client\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Proxy hostname\",\n      \"example\": \"proxy.example.com\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Proxy port\",\n      \"example\": 8080\n    },\n    \"scheme\": {\n      \"type\": \"string\",\n      \"description\": \"Proxy scheme (http or https)\",\n      \"example\": \"http\"\n    },\n    \"username\": {\n      \"type\": \"string\",\n      \"description\": \"Proxy authentication username\",\n      \"example\": \"proxyuser\"\n    },\n    \"password\": {\n      \"type\": \"string\",\n      \"description\": \"Proxy authentication password\"\
  ,\n      \"example\": \"\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-http/refs/heads/main/json-schema/http-client-proxyconfig-schema.json
tags:
- Apache
- HTTP Client
- Java
- Open Source
- SDK
title: ProxyConfig
---
