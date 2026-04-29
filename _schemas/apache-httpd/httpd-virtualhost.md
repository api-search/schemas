---
description: Apache HTTP Server virtual host configuration
layout: schema
name: VirtualHost
properties_list:
- description: Primary server name (ServerName directive)
  name: serverName
  type: string
- description: Additional server aliases
  name: serverAliases
  type: array
- description: Document root directory path
  name: documentRoot
  type: string
- description: Listening port
  name: port
  type: integer
- description: Whether SSL/TLS is enabled
  name: sslEnabled
  type: boolean
- description: Error log file path
  name: errorLog
  type: string
- description: Access log file path
  name: accessLog
  type: string
provider_name: Apache HTTP Server
provider_slug: apache-httpd
schema_file: json-schema/httpd-virtualhost-schema.json
slug: httpd-virtualhost
source_json: "{\n  \"$schema\": \"http://json-schema.org/draft-07/schema#\",\n  \"$id\": \"https://api-evangelist.github.io/apache-httpd/json-schema/httpd-virtualhost-schema.json\",\n  \"title\": \"VirtualHost\",\n  \"type\": \"object\",\n  \"description\": \"Apache HTTP Server virtual host configuration\",\n  \"properties\": {\n    \"serverName\": {\n      \"type\": \"string\",\n      \"description\": \"Primary server name (ServerName directive)\",\n      \"example\": \"www.example.com\"\n    },\n    \"serverAliases\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Additional server aliases\",\n      \"example\": [\n        \"example.com\"\n      ]\n    },\n    \"documentRoot\": {\n      \"type\": \"string\",\n      \"description\": \"Document root directory path\",\n      \"example\": \"/var/www/html\"\n    },\n    \"port\": {\n      \"type\": \"integer\",\n      \"description\": \"Listening port\",\n      \"example\"\
  : 443\n    },\n    \"sslEnabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether SSL/TLS is enabled\",\n      \"example\": true\n    },\n    \"errorLog\": {\n      \"type\": \"string\",\n      \"description\": \"Error log file path\",\n      \"example\": \"/var/log/apache2/error.log\"\n    },\n    \"accessLog\": {\n      \"type\": \"string\",\n      \"description\": \"Access log file path\",\n      \"example\": \"/var/log/apache2/access.log\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/apache-httpd/refs/heads/main/json-schema/httpd-virtualhost-schema.json
tags:
- Apache
- Load Balancer
- Open Source
- Proxy
- Reverse Proxy
- Web Server
title: VirtualHost
---
