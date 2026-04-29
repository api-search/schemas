---
description: Zone resource cap utilization statistics
layout: schema
name: ZoneCapStats
properties_list:
- description: Zone name
  name: zonename
  type: string
- description: Numeric zone ID
  name: zone_id
  type: integer
- description: CPU cap value (percentage of a CPU)
  name: cpu_cap
  type: number
- description: Current CPU usage percentage
  name: cpu_usage
  type: number
- description: Number of times zone waited due to CPU cap
  name: cpu_nwait
  type: integer
- description: Physical memory cap in bytes
  name: memory_cap
  type: integer
- description: Current physical memory usage in bytes
  name: memory_usage
  type: integer
- description: Swap cap in bytes
  name: swap_cap
  type: integer
- description: Current swap usage in bytes
  name: swap_usage
  type: integer
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-stats-zone-cap-stats-schema.json
slug: solaris-zone-stats-zone-cap-stats
source_filename: solaris-zone-stats-zone-cap-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZoneCapStats\",\n  \"type\": \"object\",\n  \"description\": \"Zone resource cap utilization statistics\",\n  \"properties\": {\n    \"zonename\": {\n      \"type\": \"string\",\n      \"description\": \"Zone name\"\n    },\n    \"zone_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric zone ID\"\n    },\n    \"cpu_cap\": {\n      \"type\": \"number\",\n      \"description\": \"CPU cap value (percentage of a CPU)\"\n    },\n    \"cpu_usage\": {\n      \"type\": \"number\",\n      \"description\": \"Current CPU usage percentage\"\n    },\n    \"cpu_nwait\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times zone waited due to CPU cap\"\n    },\n    \"memory_cap\": {\n      \"type\": \"integer\",\n      \"description\": \"Physical memory cap in bytes\"\n    },\n    \"memory_usage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current physical\
  \ memory usage in bytes\"\n    },\n    \"swap_cap\": {\n      \"type\": \"integer\",\n      \"description\": \"Swap cap in bytes\"\n    },\n    \"swap_usage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current swap usage in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-stats-zone-cap-stats-schema.json
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
title: ZoneCapStats
---
