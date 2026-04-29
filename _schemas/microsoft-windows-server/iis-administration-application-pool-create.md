---
description: Request body for creating a new application pool.
layout: schema
name: ApplicationPoolCreate
properties_list:
- description: The name of the application pool to create.
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
schema_file: json-schema/iis-administration-application-pool-create-schema.json
slug: iis-administration-application-pool-create
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationPoolCreate\",\n  \"type\": \"object\",\n  \"description\": \"Request body for creating a new application pool.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application pool to create.\"\n    },\n    \"auto_start\": {\n      \"type\": \"boolean\"\n    },\n    \"pipeline_mode\": {\n      \"type\": \"string\"\n    },\n    \"managed_runtime_version\": {\n      \"type\": \"string\"\n    },\n    \"enable_32bit_win64\": {\n      \"type\": \"boolean\"\n    },\n    \"queue_length\": {\n      \"type\": \"integer\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-application-pool-create-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ApplicationPoolCreate
---
