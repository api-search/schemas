---
description: Zone miscellaneous statistics
layout: schema
name: ZoneMiscStats
properties_list:
- description: ''
  name: zonename
  type: string
- description: ''
  name: zone_id
  type: integer
- description: Number of processes in the zone
  name: nprocs
  type: integer
- description: Number of lightweight processes in the zone
  name: nlwps
  type: integer
- description: Total process size in bytes
  name: pr_size
  type: integer
- description: Total resident set size in bytes
  name: pr_rss
  type: integer
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-stats-zone-misc-stats-schema.json
slug: solaris-zone-stats-zone-misc-stats
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ZoneMiscStats\",\n  \"type\": \"object\",\n  \"description\": \"Zone miscellaneous statistics\",\n  \"properties\": {\n    \"zonename\": {\n      \"type\": \"string\"\n    },\n    \"zone_id\": {\n      \"type\": \"integer\"\n    },\n    \"nprocs\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of processes in the zone\"\n    },\n    \"nlwps\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of lightweight processes in the zone\"\n    },\n    \"pr_size\": {\n      \"type\": \"integer\",\n      \"description\": \"Total process size in bytes\"\n    },\n    \"pr_rss\": {\n      \"type\": \"integer\",\n      \"description\": \"Total resident set size in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-stats-zone-misc-stats-schema.json
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
title: ZoneMiscStats
---
