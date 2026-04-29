---
description: A summary representation of a web site in list responses.
layout: schema
name: WebSiteSummary
properties_list:
- description: The name of the web site.
  name: name
  type: string
- description: The unique identifier of the web site.
  name: id
  type: string
- description: The current status of the web site.
  name: status
  type: string
- description: ''
  name: _links
  type: object
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-web-site-summary-schema.json
slug: iis-administration-web-site-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebSiteSummary\",\n  \"type\": \"object\",\n  \"description\": \"A summary representation of a web site in list responses.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the web site.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the web site.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the web site.\"\n    },\n    \"_links\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-web-site-summary-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: WebSiteSummary
---
