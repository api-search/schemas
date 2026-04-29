---
description: Recycling settings for the application pool.
layout: schema
name: Recycling
properties_list:
- description: Whether to disable overlapped recycling.
  name: disable_overlapped_recycle
  type: boolean
- description: Whether to disable recycling on configuration changes.
  name: disable_recycle_on_config_change
  type: boolean
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-recycling-schema.json
slug: iis-administration-recycling
source_filename: iis-administration-recycling-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Recycling\",\n  \"type\": \"object\",\n  \"description\": \"Recycling settings for the application pool.\",\n  \"properties\": {\n    \"disable_overlapped_recycle\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable overlapped recycling.\"\n    },\n    \"disable_recycle_on_config_change\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether to disable recycling on configuration changes.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-recycling-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: Recycling
---
