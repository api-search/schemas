---
description: ''
layout: schema
name: SystemMemoryStats
properties_list:
- description: Total physical memory pages
  name: physmem
  type: integer
- description: Free memory pages
  name: freemem
  type: integer
- description: Available real memory pages
  name: availrmem
  type: integer
- description: Lotsfree threshold
  name: lotsfree
  type: integer
- description: Desfree threshold
  name: desfree
  type: integer
- description: Minfree threshold
  name: minfree
  type: integer
- description: Pages used by kernel
  name: pp_kernel
  type: integer
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-stats-system-memory-stats-schema.json
slug: solaris-zone-stats-system-memory-stats
source_filename: solaris-zone-stats-system-memory-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SystemMemoryStats\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"physmem\": {\n      \"type\": \"integer\",\n      \"description\": \"Total physical memory pages\"\n    },\n    \"freemem\": {\n      \"type\": \"integer\",\n      \"description\": \"Free memory pages\"\n    },\n    \"availrmem\": {\n      \"type\": \"integer\",\n      \"description\": \"Available real memory pages\"\n    },\n    \"lotsfree\": {\n      \"type\": \"integer\",\n      \"description\": \"Lotsfree threshold\"\n    },\n    \"desfree\": {\n      \"type\": \"integer\",\n      \"description\": \"Desfree threshold\"\n    },\n    \"minfree\": {\n      \"type\": \"integer\",\n      \"description\": \"Minfree threshold\"\n    },\n    \"pp_kernel\": {\n      \"type\": \"integer\",\n      \"description\": \"Pages used by kernel\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-stats-system-memory-stats-schema.json
tags:
- Containers
- Kernel Zones
- Operating Systems
- Oracle
- RAD
- Resource Management
- Solaris
- StatsStore
- Virtualization
- Zones
title: SystemMemoryStats
---
