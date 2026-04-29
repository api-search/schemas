---
description: Swap cap statistics
layout: schema
name: SwapCapStats
properties_list:
- description: Swap cap in bytes
  name: swapcap
  type: integer
- description: Current swap usage in bytes
  name: usage
  type: integer
- description: Number of times swap exceeded the cap
  name: nover
  type: integer
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-stats-swap-cap-stats-schema.json
slug: solaris-zone-stats-swap-cap-stats
source_filename: solaris-zone-stats-swap-cap-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"SwapCapStats\",\n  \"type\": \"object\",\n  \"description\": \"Swap cap statistics\",\n  \"properties\": {\n    \"swapcap\": {\n      \"type\": \"integer\",\n      \"description\": \"Swap cap in bytes\"\n    },\n    \"usage\": {\n      \"type\": \"integer\",\n      \"description\": \"Current swap usage in bytes\"\n    },\n    \"nover\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of times swap exceeded the cap\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-stats-swap-cap-stats-schema.json
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
title: SwapCapStats
---
