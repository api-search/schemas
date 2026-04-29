---
description: Request body for updating a web site. Only include properties that should be changed. Note that list properties like bindings replace the entire list.
layout: schema
name: WebSiteUpdate
properties_list:
- description: The name of the web site.
  name: name
  type: string
- description: The physical file system path for the web site root.
  name: physical_path
  type: string
- description: The full list of desired bindings. Existing bindings not included in this list will be removed.
  name: bindings
  type: array
- description: ''
  name: application_pool
  type: object
- description: ''
  name: server_auto_start
  type: boolean
- description: ''
  name: enabled_protocols
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-web-site-update-schema.json
slug: iis-administration-web-site-update
source_filename: iis-administration-web-site-update-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"WebSiteUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating a web site. Only include properties that should be changed. Note that list properties like bindings replace the entire list.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the web site.\"\n    },\n    \"physical_path\": {\n      \"type\": \"string\",\n      \"description\": \"The physical file system path for the web site root.\"\n    },\n    \"bindings\": {\n      \"type\": \"array\",\n      \"description\": \"The full list of desired bindings. Existing bindings not included in this list will be removed.\"\n    },\n    \"application_pool\": {\n      \"type\": \"object\"\n    },\n    \"server_auto_start\": {\n      \"type\": \"boolean\"\n    },\n    \"enabled_protocols\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-web-site-update-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: WebSiteUpdate
---
