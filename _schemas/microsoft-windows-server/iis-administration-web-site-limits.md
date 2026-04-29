---
description: Resource limits for the web site.
layout: schema
name: WebSiteLimits
properties_list:
- description: The connection timeout in seconds.
  name: connection_timeout
  type: integer
- description: The maximum bandwidth in bytes per second.
  name: max_bandwidth
  type: integer
- description: The maximum number of concurrent connections.
  name: max_connections
  type: integer
- description: The maximum number of URL segments allowed.
  name: max_url_segments
  type: integer
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-web-site-limits-schema.json
slug: iis-administration-web-site-limits
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebSiteLimits\",\n  \"type\": \"object\",\n  \"description\": \"Resource limits for the web site.\",\n  \"properties\": {\n    \"connection_timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"The connection timeout in seconds.\"\n    },\n    \"max_bandwidth\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum bandwidth in bytes per second.\"\n    },\n    \"max_connections\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of concurrent connections.\"\n    },\n    \"max_url_segments\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of URL segments allowed.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-web-site-limits-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: WebSiteLimits
---
