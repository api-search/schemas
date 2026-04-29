---
description: Periodic restart configuration for the application pool.
layout: schema
name: PeriodicRestart
properties_list:
- description: The time interval in minutes after which the application pool recycles.
  name: time_interval
  type: integer
- description: The private memory threshold in kilobytes that triggers recycling. 0 means disabled.
  name: private_memory
  type: integer
- description: The number of requests after which the application pool recycles. 0 means disabled.
  name: request_limit
  type: integer
- description: The virtual memory threshold in kilobytes that triggers recycling. 0 means disabled.
  name: virtual_memory
  type: integer
- description: Scheduled times for recycling the application pool.
  name: schedule
  type: array
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-periodic-restart-schema.json
slug: iis-administration-periodic-restart
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PeriodicRestart\",\n  \"type\": \"object\",\n  \"description\": \"Periodic restart configuration for the application pool.\",\n  \"properties\": {\n    \"time_interval\": {\n      \"type\": \"integer\",\n      \"description\": \"The time interval in minutes after which the application pool recycles.\"\n    },\n    \"private_memory\": {\n      \"type\": \"integer\",\n      \"description\": \"The private memory threshold in kilobytes that triggers recycling. 0 means disabled.\"\n    },\n    \"request_limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The number of requests after which the application pool recycles. 0 means disabled.\"\n    },\n    \"virtual_memory\": {\n      \"type\": \"integer\",\n      \"description\": \"The virtual memory threshold in kilobytes that triggers recycling. 0 means disabled.\"\n    },\n    \"schedule\": {\n      \"type\": \"array\",\n      \"description\"\
  : \"Scheduled times for recycling the application pool.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-periodic-restart-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: PeriodicRestart
---
