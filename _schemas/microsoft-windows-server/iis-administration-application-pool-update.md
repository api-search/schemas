---
description: Request body for updating an application pool. Only include properties that should be changed.
layout: schema
name: ApplicationPoolUpdate
properties_list:
- description: ''
  name: name
  type: string
- description: ''
  name: auto_start
  type: boolean
- description: ''
  name: pipeline_mode
  type: string
- description: ''
  name: managed_runtime_version
  type: string
- description: ''
  name: enable_32bit_win64
  type: boolean
- description: ''
  name: queue_length
  type: integer
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-application-pool-update-schema.json
slug: iis-administration-application-pool-update
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationPoolUpdate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for updating an application pool. Only include properties that should be changed.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\"\n    },\n    \"auto_start\": {\n      \"type\": \"boolean\"\n    },\n    \"pipeline_mode\": {\n      \"type\": \"string\"\n    },\n    \"managed_runtime_version\": {\n      \"type\": \"string\"\n    },\n    \"enable_32bit_win64\": {\n      \"type\": \"boolean\"\n    },\n    \"queue_length\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-application-pool-update-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ApplicationPoolUpdate
---
