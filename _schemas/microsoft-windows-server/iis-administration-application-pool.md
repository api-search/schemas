---
description: A complete IIS application pool resource with all configuration settings for worker process isolation and management.
layout: schema
name: ApplicationPool
properties_list:
- description: The name of the application pool.
  name: name
  type: string
- description: The unique identifier of the application pool.
  name: id
  type: string
- description: The current status of the application pool.
  name: status
  type: string
- description: Whether the application pool starts automatically when IIS starts.
  name: auto_start
  type: boolean
- description: The managed pipeline mode for the application pool.
  name: pipeline_mode
  type: string
- description: The version of the .NET CLR loaded by the application pool. Empty string for unmanaged code.
  name: managed_runtime_version
  type: string
- description: Whether to enable 32-bit applications on 64-bit Windows.
  name: enable_32bit_win64
  type: boolean
- description: The maximum number of requests that can be queued for the application pool before requests are rejected.
  name: queue_length
  type: integer
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-application-pool-schema.json
slug: iis-administration-application-pool
source_filename: iis-administration-application-pool-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ApplicationPool\",\n  \"type\": \"object\",\n  \"description\": \"A complete IIS application pool resource with all configuration settings for worker process isolation and management.\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the application pool.\"\n    },\n    \"id\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the application pool.\"\n    },\n    \"status\": {\n      \"type\": \"string\",\n      \"description\": \"The current status of the application pool.\"\n    },\n    \"auto_start\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the application pool starts automatically when IIS starts.\"\n    },\n    \"pipeline_mode\": {\n      \"type\": \"string\",\n      \"description\": \"The managed pipeline mode for the application pool.\"\n    },\n    \"managed_runtime_version\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The version of the .NET CLR loaded by the application pool. Empty string for unmanaged code.\"\n    },\n    \"enable_32bit_win64\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to enable 32-bit applications on 64-bit Windows.\"\n    },\n    \"queue_length\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of requests that can be queued for the application pool before requests are rejected.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-application-pool-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ApplicationPool
---
