---
description: Represents resource utilization statistics for an Oracle Solaris Zone, including CPU, memory, swap, and process metrics collected via the kstat interface and libzonestat library.
layout: schema
name: Oracle Solaris Zone Statistics
properties_list:
- description: Name of the zone
  name: zonename
  type: string
- description: Numeric zone identifier
  name: zone_id
  type: integer
- description: CPU cap value as a percentage of a single CPU (100 = 1 full CPU)
  name: cpu_cap
  type: number
- description: Current CPU usage as a percentage
  name: cpu_usage
  type: number
- description: Number of times zone threads waited due to CPU cap
  name: cpu_nwait
  type: integer
- description: Physical memory cap in bytes
  name: memory_cap
  type: integer
- description: Current physical memory usage (RSS) in bytes
  name: memory_usage
  type: integer
- description: Swap space cap in bytes
  name: swap_cap
  type: integer
- description: Current swap space usage in bytes
  name: swap_usage
  type: integer
- description: Number of processes running in the zone
  name: nprocs
  type: integer
- description: Number of lightweight processes (threads) in the zone
  name: nlwps
  type: integer
- description: Total virtual size of all processes in bytes
  name: pr_size
  type: integer
- description: Total resident set size of all processes in bytes
  name: pr_rss
  type: integer
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-stats-schema.json
slug: solaris-zone-stats
source_filename: solaris-zone-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://docs.oracle.com/schemas/solaris/zone-stats.json\",\n  \"title\": \"Oracle Solaris Zone Statistics\",\n  \"description\": \"Represents resource utilization statistics for an Oracle Solaris Zone, including CPU, memory, swap, and process metrics collected via the kstat interface and libzonestat library.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"zonename\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the zone\"\n    },\n    \"zone_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Numeric zone identifier\",\n      \"minimum\": 0\n    },\n    \"cpu_cap\": {\n      \"type\": \"number\",\n      \"description\": \"CPU cap value as a percentage of a single CPU (100 = 1 full CPU)\",\n      \"minimum\": 0\n    },\n    \"cpu_usage\": {\n      \"type\": \"number\",\n      \"description\": \"Current CPU usage as a percentage\",\n      \"minimum\": 0\n\
  \    },\n    \"cpu_nwait\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times zone threads waited due to CPU cap\",\n      \"minimum\": 0\n    },\n    \"memory_cap\": {\n      \"type\": \"integer\",\n      \"description\": \"Physical memory cap in bytes\",\n      \"minimum\": 0\n    },\n    \"memory_usage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current physical memory usage (RSS) in bytes\",\n      \"minimum\": 0\n    },\n    \"swap_cap\": {\n      \"type\": \"integer\",\n      \"description\": \"Swap space cap in bytes\",\n      \"minimum\": 0\n    },\n    \"swap_usage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current swap space usage in bytes\",\n      \"minimum\": 0\n    },\n    \"nprocs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of processes running in the zone\",\n      \"minimum\": 0\n    },\n    \"nlwps\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of lightweight processes\
  \ (threads) in the zone\",\n      \"minimum\": 0\n    },\n    \"pr_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Total virtual size of all processes in bytes\",\n      \"minimum\": 0\n    },\n    \"pr_rss\": {\n      \"type\": \"integer\",\n      \"description\": \"Total resident set size of all processes in bytes\",\n      \"minimum\": 0\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-stats-schema.json
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
title: Oracle Solaris Zone Statistics
---
