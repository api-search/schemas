---
description: Configuration for which recycling events are logged.
layout: schema
name: RecyclingLogEvents
properties_list:
- description: ''
  name: time
  type: boolean
- description: ''
  name: requests
  type: boolean
- description: ''
  name: schedule
  type: boolean
- description: ''
  name: memory
  type: boolean
- description: ''
  name: isapi_unhealthy
  type: boolean
- description: ''
  name: on_demand
  type: boolean
- description: ''
  name: config_change
  type: boolean
- description: ''
  name: private_memory
  type: boolean
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
schema_file: json-schema/iis-administration-recycling-log-events-schema.json
slug: iis-administration-recycling-log-events
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"RecyclingLogEvents\",\n  \"type\": \"object\",\n  \"description\": \"Configuration for which recycling events are logged.\",\n  \"properties\": {\n    \"time\": {\n      \"type\": \"boolean\"\n    },\n    \"requests\": {\n      \"type\": \"boolean\"\n    },\n    \"schedule\": {\n      \"type\": \"boolean\"\n    },\n    \"memory\": {\n      \"type\": \"boolean\"\n    },\n    \"isapi_unhealthy\": {\n      \"type\": \"boolean\"\n    },\n    \"on_demand\": {\n      \"type\": \"boolean\"\n    },\n    \"config_change\": {\n      \"type\": \"boolean\"\n    },\n    \"private_memory\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-windows-server/refs/heads/main/json-schema/iis-administration-recycling-log-events-schema.json
tags:
- Datacenter
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
title: RecyclingLogEvents
---
