---
description: ''
layout: schema
name: VmCpuStats
properties_list:
- description: Nanoseconds spent idle
  name: cpu_nsec_idle
  type: integer
- description: Nanoseconds spent in kernel mode
  name: cpu_nsec_kernel
  type: integer
- description: Nanoseconds spent in user mode
  name: cpu_nsec_user
  type: integer
- description: Nanoseconds spent in DTrace
  name: cpu_nsec_dtrace
  type: integer
- description: Nanoseconds spent handling interrupts
  name: cpu_nsec_intr
  type: integer
provider_name: Solaris Zones
provider_slug: solaris-zones
schema_file: json-schema/solaris-zone-monitoring-vm-cpu-stats-schema.json
slug: solaris-zone-monitoring-vm-cpu-stats
source_filename: solaris-zone-monitoring-vm-cpu-stats-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VmCpuStats\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"cpu_nsec_idle\": {\n      \"type\": \"integer\",\n      \"description\": \"Nanoseconds spent idle\"\n    },\n    \"cpu_nsec_kernel\": {\n      \"type\": \"integer\",\n      \"description\": \"Nanoseconds spent in kernel mode\"\n    },\n    \"cpu_nsec_user\": {\n      \"type\": \"integer\",\n      \"description\": \"Nanoseconds spent in user mode\"\n    },\n    \"cpu_nsec_dtrace\": {\n      \"type\": \"integer\",\n      \"description\": \"Nanoseconds spent in DTrace\"\n    },\n    \"cpu_nsec_intr\": {\n      \"type\": \"integer\",\n      \"description\": \"Nanoseconds spent handling interrupts\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/solaris-zones/refs/heads/main/json-schema/solaris-zone-monitoring-vm-cpu-stats-schema.json
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
title: VmCpuStats
---
