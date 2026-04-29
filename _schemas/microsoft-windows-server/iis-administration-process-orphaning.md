---
description: Process orphaning settings that control behavior when a worker process cannot be shut down gracefully.
layout: schema
name: ProcessOrphaning
properties_list:
- description: Whether process orphaning is enabled.
  name: enabled
  type: boolean
- description: The path to an executable to run when a worker process is orphaned.
  name: orphan_action_exe
  type: string
- description: Parameters for the orphan action executable.
  name: orphan_action_params
  type: string
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-process-orphaning-schema.json
slug: iis-administration-process-orphaning
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ProcessOrphaning\",\n  \"type\": \"object\",\n  \"description\": \"Process orphaning settings that control behavior when a worker process cannot be shut down gracefully.\",\n  \"properties\": {\n    \"enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether process orphaning is enabled.\"\n    },\n    \"orphan_action_exe\": {\n      \"type\": \"string\",\n      \"description\": \"The path to an executable to run when a worker process is orphaned.\"\n    },\n    \"orphan_action_params\": {\n      \"type\": \"string\",\n      \"description\": \"Parameters for the orphan action executable.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-process-orphaning-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: ProcessOrphaning
---
