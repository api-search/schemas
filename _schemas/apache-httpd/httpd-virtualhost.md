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
tags:
- Apache
- Load Balancer
- Open Source
- Proxy
- Reverse Proxy
- Web Server
title: VirtualHost
---
