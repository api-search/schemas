---
description: CPU cap statistics
layout: schema
name: CpuCapStats
properties_list:
- description: CPU cap value in microseconds per second
  name: value
  type: integer
- description: Current CPU usage in microseconds per second
  name: usage
  type: integer
- description: Number of times threads waited due to cap
  name: nwait
  type: integer
- description: Time spent below the cap in nanoseconds
  name: below
  type: integer
- description: Time spent above the cap in nanoseconds
  name: above
  type: integer
- description: Maximum CPU usage observed
  name: maxusage
  type: integer
- description: Zone name
  name: zonename
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-stats-cpu-cap-stats-schema.json
slug: solaris-zone-stats-cpu-cap-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CpuCapStats\",\n  \"type\": \"object\",\n  \"description\": \"CPU cap statistics\",\n  \"properties\": {\n    \"value\": {\n      \"type\": \"integer\",\n      \"description\": \"CPU cap value in microseconds per second\"\n    },\n    \"usage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current CPU usage in microseconds per second\"\n    },\n    \"nwait\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times threads waited due to cap\"\n    },\n    \"below\": {\n      \"type\": \"integer\",\n      \"description\": \"Time spent below the cap in nanoseconds\"\n    },\n    \"above\": {\n      \"type\": \"integer\",\n      \"description\": \"Time spent above the cap in nanoseconds\"\n    },\n    \"maxusage\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum CPU usage observed\"\n    },\n    \"zonename\": {\n      \"type\": \"string\",\n     \
  \ \"description\": \"Zone name\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-stats-cpu-cap-stats-schema.json
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
title: CpuCapStats
---
