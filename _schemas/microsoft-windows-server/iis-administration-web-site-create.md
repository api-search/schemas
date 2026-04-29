---
description: Request body for creating a new web site.
layout: schema
name: WebSiteCreate
properties_list:
- description: The name of the web site to create.
  name: name
  type: string
- description: The physical file system path for the web site root directory. The directory must exist.
  name: physical_path
  type: string
- description: The bindings for the web site.
  name: bindings
  type: array
- description: Optional application pool assignment.
  name: application_pool
  type: object
- description: Whether the web site starts automatically when IIS starts.
  name: server_auto_start
  type: boolean
- description: The protocols enabled for this web site.
  name: enabled_protocols
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-web-site-create-schema.json
slug: iis-administration-web-site-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebSiteCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new web site.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the web site to create.\"\n    },\n    \"physical_path\": {\n      \"type\": \"string\",\n      \"description\": \"The physical file system path for the web site root directory. The directory must exist.\"\n    },\n    \"bindings\": {\n      \"type\": \"array\",\n      \"description\": \"The bindings for the web site.\"\n    },\n    \"application_pool\": {\n      \"type\": \"object\",\n      \"description\": \"Optional application pool assignment.\"\n    },\n    \"server_auto_start\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the web site starts automatically when IIS starts.\"\n    },\n    \"enabled_protocols\": {\n      \"type\": \"string\",\n      \"description\"\
  : \"The protocols enabled for this web site.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-web-site-create-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: WebSiteCreate
---
