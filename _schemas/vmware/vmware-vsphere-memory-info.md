---
description: Memory configuration of a virtual machine
layout: schema
name: MemoryInfo
properties_list:
- description: Memory size in mebibytes
  name: size_MiB
  type: integer
- description: Whether memory hot-add is enabled
  name: hot_add_enabled
  type: boolean
- description: Granularity for memory hot-add in mebibytes
  name: hot_add_increment_size_MiB
  type: integer
- description: Maximum memory size for hot-add in mebibytes
  name: hot_add_limit_MiB
  type: integer
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-memory-info-schema.json
slug: vmware-vsphere-memory-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemoryInfo\",\n  \"type\": \"object\",\n  \"description\": \"Memory configuration of a virtual machine\",\n  \"properties\": {\n    \"size_MiB\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory size in mebibytes\"\n    },\n    \"hot_add_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether memory hot-add is enabled\"\n    },\n    \"hot_add_increment_size_MiB\": {\n      \"type\": \"integer\",\n      \"description\": \"Granularity for memory hot-add in mebibytes\"\n    },\n    \"hot_add_limit_MiB\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum memory size for hot-add in mebibytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-memory-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: MemoryInfo
---
