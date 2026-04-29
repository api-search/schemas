---
description: ''
layout: schema
name: CpuInfo
properties_list:
- description: CPU brand string
  name: brand
  type: string
- description: ''
  name: chip_id
  type: integer
- description: ''
  name: clock_MHz
  type: integer
- description: ''
  name: core_id
  type: integer
- description: ''
  name: cpu_type
  type: string
- description: ''
  name: implementation
  type: string
- description: ''
  name: ncore_per_chip
  type: integer
- description: ''
  name: state
  type: string
- description: ''
  name: vendor_id
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-stats-cpu-info-schema.json
slug: solaris-zone-stats-cpu-info
source_filename: solaris-zone-stats-cpu-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CpuInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"CPU brand string\"\n    },\n    \"chip_id\": {\n      \"type\": \"integer\"\n    },\n    \"clock_MHz\": {\n      \"type\": \"integer\"\n    },\n    \"core_id\": {\n      \"type\": \"integer\"\n    },\n    \"cpu_type\": {\n      \"type\": \"string\"\n    },\n    \"implementation\": {\n      \"type\": \"string\"\n    },\n    \"ncore_per_chip\": {\n      \"type\": \"integer\"\n    },\n    \"state\": {\n      \"type\": \"string\"\n    },\n    \"vendor_id\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-stats-cpu-info-schema.json
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
title: CpuInfo
---
