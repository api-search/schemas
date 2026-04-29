---
description: CPU usage settings for the application pool.
layout: schema
name: CpuSettings
properties_list:
- description: The maximum CPU usage percentage (in 1/1000ths of a percent) allowed for the application pool.
  name: limit
  type: integer
- description: The interval in minutes for CPU limit monitoring.
  name: limit_interval
  type: integer
- description: The action to take when the CPU limit is exceeded.
  name: action
  type: string
- description: Whether processor affinity is enabled.
  name: processor_affinity_enabled
  type: boolean
- description: The 32-bit processor affinity mask.
  name: processor_affinity_mask32
  type: string
- description: The 64-bit processor affinity mask.
  name: processor_affinity_mask64
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-cpu-settings-schema.json
slug: iis-administration-cpu-settings
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CpuSettings\",\n  \"type\": \"object\",\n  \"description\": \"CPU usage settings for the application pool.\",\n  \"properties\": {\n    \"limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum CPU usage percentage (in 1/1000ths of a percent) allowed for the application pool.\"\n    },\n    \"limit_interval\": {\n      \"type\": \"integer\",\n      \"description\": \"The interval in minutes for CPU limit monitoring.\"\n    },\n    \"action\": {\n      \"type\": \"string\",\n      \"description\": \"The action to take when the CPU limit is exceeded.\"\n    },\n    \"processor_affinity_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether processor affinity is enabled.\"\n    },\n    \"processor_affinity_mask32\": {\n      \"type\": \"string\",\n      \"description\": \"The 32-bit processor affinity mask.\"\n    },\n    \"processor_affinity_mask64\"\
  : {\n      \"type\": \"string\",\n      \"description\": \"The 64-bit processor affinity mask.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-cpu-settings-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: CpuSettings
---
