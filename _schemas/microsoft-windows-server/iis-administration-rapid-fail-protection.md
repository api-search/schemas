---
description: Rapid fail protection settings that determine how IIS responds to repeated worker process failures.
layout: schema
name: RapidFailProtection
properties_list:
- description: Whether rapid fail protection is enabled.
  name: enabled
  type: boolean
- description: The load balancer capabilities response type.
  name: load_balancer_capabilities
  type: string
- description: The time interval in minutes during which the max crash count is monitored.
  name: interval
  type: integer
- description: The maximum number of worker process crashes allowed within the interval.
  name: max_crashes
  type: integer
- description: The path to an executable to run when the application pool is shut down due to rapid fail protection.
  name: auto_shutdown_exe
  type: string
- description: Parameters for the auto shutdown executable.
  name: auto_shutdown_params
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-rapid-fail-protection-schema.json
slug: iis-administration-rapid-fail-protection
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RapidFailProtection\",\n  \"type\": \"object\",\n  \"description\": \"Rapid fail protection settings that determine how IIS responds to repeated worker process failures.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether rapid fail protection is enabled.\"\n    },\n    \"load_balancer_capabilities\": {\n      \"type\": \"string\",\n      \"description\": \"The load balancer capabilities response type.\"\n    },\n    \"interval\": {\n      \"type\": \"integer\",\n      \"description\": \"The time interval in minutes during which the max crash count is monitored.\"\n    },\n    \"max_crashes\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of worker process crashes allowed within the interval.\"\n    },\n    \"auto_shutdown_exe\": {\n      \"type\": \"string\",\n      \"description\": \"The path to an executable\
  \ to run when the application pool is shut down due to rapid fail protection.\"\n    },\n    \"auto_shutdown_params\": {\n      \"type\": \"string\",\n      \"description\": \"Parameters for the auto shutdown executable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-rapid-fail-protection-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: RapidFailProtection
---
