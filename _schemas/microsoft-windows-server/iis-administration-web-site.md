---
description: A complete IIS web site resource including configuration, bindings, application pool assignment, and HAL links to related resources.
layout: schema
name: WebSite
properties_list:
- description: The name of the web site.
  name: name
  type: string
- description: The unique identifier of the web site.
  name: id
  type: string
- description: The physical file system path for the web site root.
  name: physical_path
  type: string
- description: The IIS site key identifier.
  name: key
  type: string
- description: The current status of the web site.
  name: status
  type: string
- description: Whether the web site starts automatically when IIS starts.
  name: server_auto_start
  type: boolean
- description: The protocols enabled for this web site, as a comma-separated list.
  name: enabled_protocols
  type: string
- description: The list of bindings configured for this web site.
  name: bindings
  type: array
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-web-site-schema.json
slug: iis-administration-web-site
source_filename: iis-administration-web-site-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebSite\",\n  \"type\": \"object\",\n  \"description\": \"A complete IIS web site resource including configuration, bindings, application pool assignment, and HAL links to related resources.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the web site.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the web site.\"\n    },\n    \"physical_path\": {\n      \"type\": \"string\",\n      \"description\": \"The physical file system path for the web site root.\"\n    },\n    \"key\": {\n      \"type\": \"string\",\n      \"description\": \"The IIS site key identifier.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the web site.\"\n    },\n    \"server_auto_start\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the web site starts automatically when IIS starts.\"\n    },\n    \"enabled_protocols\": {\n      \"type\": \"string\",\n      \"description\": \"The protocols enabled for this web site, as a comma-separated list.\"\n    },\n    \"bindings\": {\n      \"type\": \"array\",\n      \"description\": \"The list of bindings configured for this web site.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-web-site-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: WebSite
---
