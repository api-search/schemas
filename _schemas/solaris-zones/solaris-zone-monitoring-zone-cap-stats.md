---
description: ''
layout: schema
name: ZoneCapStats
properties_list:
- description: Zone name
  name: zonename
  type: string
- description: Numeric zone ID
  name: zone_id
  type: integer
- description: CPU cap value
  name: cpu_cap
  type: number
- description: Current CPU usage
  name: cpu_usage
  type: number
- description: Memory cap in bytes
  name: memory_cap
  type: integer
- description: Current memory usage in bytes
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
schema_file: json-schema/solaris-zone-monitoring-zone-cap-stats-schema.json
slug: solaris-zone-monitoring-zone-cap-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZoneCapStats\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"zonename\": {\n      \"type\": \"string\",\n      \"description\": \"Zone name\"\n    },\n    \"zone_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric zone ID\"\n    },\n    \"cpu_cap\": {\n      \"type\": \"number\",\n      \"description\": \"CPU cap value\"\n    },\n    \"cpu_usage\": {\n      \"type\": \"number\",\n      \"description\": \"Current CPU usage\"\n    },\n    \"memory_cap\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory cap in bytes\"\n    },\n    \"memory_usage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current memory usage in bytes\"\n    },\n    \"swap_cap\": {\n      \"type\": \"integer\",\n      \"description\": \"Swap cap in bytes\"\n    },\n    \"swap_usage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current swap usage in bytes\"\
  \n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-monitoring-zone-cap-stats-schema.json
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
