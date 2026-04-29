---
description: Process model settings for the application pool worker processes.
layout: schema
name: ProcessModel
properties_list:
- description: The idle timeout in minutes before a worker process is shut down.
  name: idle_timeout
  type: integer
- description: The maximum number of worker processes for the application pool (web garden).
  name: max_processes
  type: integer
- description: Whether health monitoring pings are enabled.
  name: pinging_enabled
  type: boolean
- description: The interval in seconds between health monitoring pings.
  name: ping_interval
  type: integer
- description: The maximum time in seconds allowed for a worker process to respond to a health ping.
  name: ping_response_time
  type: integer
- description: The time in seconds allowed for a worker process to gracefully shut down.
  name: shutdown_time_limit
  type: integer
- description: The time in seconds allowed for a worker process to start up.
  name: startup_time_limit
  type: integer
- description: The action to take when the idle timeout is reached.
  name: idle_timeout_action
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-process-model-schema.json
slug: iis-administration-process-model
source_filename: iis-administration-process-model-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProcessModel\",\n  \"type\": \"object\",\n  \"description\": \"Process model settings for the application pool worker processes.\",\n  \"properties\": {\n    \"idle_timeout\": {\n      \"type\": \"integer\",\n      \"description\": \"The idle timeout in minutes before a worker process is shut down.\"\n    },\n    \"max_processes\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of worker processes for the application pool (web garden).\"\n    },\n    \"pinging_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether health monitoring pings are enabled.\"\n    },\n    \"ping_interval\": {\n      \"type\": \"integer\",\n      \"description\": \"The interval in seconds between health monitoring pings.\"\n    },\n    \"ping_response_time\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum time in seconds allowed for a worker\
  \ process to respond to a health ping.\"\n    },\n    \"shutdown_time_limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The time in seconds allowed for a worker process to gracefully shut down.\"\n    },\n    \"startup_time_limit\": {\n      \"type\": \"integer\",\n      \"description\": \"The time in seconds allowed for a worker process to start up.\"\n    },\n    \"idle_timeout_action\": {\n      \"type\": \"string\",\n      \"description\": \"The action to take when the idle timeout is reached.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-process-model-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ProcessModel
---
