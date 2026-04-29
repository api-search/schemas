---
description: ''
layout: schema
name: CpuInfo
properties_list:
- description: CPU brand string
  name: brand
  type: string
- description: Physical chip ID
  name: chip_id
  type: integer
- description: CPU clock speed in MHz
  name: clock_MHz
  type: integer
- description: Core ID within the chip
  name: core_id
  type: integer
- description: CPU type identifier
  name: cpu_type
  type: string
- description: CPU implementation description
  name: implementation
  type: string
- description: Number of cores per chip
  name: ncore_per_chip
  type: integer
- description: CPU state (on-line, off-line)
  name: state
  type: string
- description: CPU vendor identifier
  name: vendor_id
  type: string
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-monitoring-cpu-info-schema.json
slug: solaris-zone-monitoring-cpu-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CpuInfo\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"brand\": {\n      \"type\": \"string\",\n      \"description\": \"CPU brand string\"\n    },\n    \"chip_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Physical chip ID\"\n    },\n    \"clock_MHz\": {\n      \"type\": \"integer\",\n      \"description\": \"CPU clock speed in MHz\"\n    },\n    \"core_id\": {\n      \"type\": \"integer\",\n      \"description\": \"Core ID within the chip\"\n    },\n    \"cpu_type\": {\n      \"type\": \"string\",\n      \"description\": \"CPU type identifier\"\n    },\n    \"implementation\": {\n      \"type\": \"string\",\n      \"description\": \"CPU implementation description\"\n    },\n    \"ncore_per_chip\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of cores per chip\"\n    },\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"CPU\
  \ state (on-line, off-line)\"\n    },\n    \"vendor_id\": {\n      \"type\": \"string\",\n      \"description\": \"CPU vendor identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-monitoring-cpu-info-schema.json
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
