---
description: CPU configuration of a virtual machine
layout: schema
name: CpuInfo
properties_list:
- description: Number of virtual CPU cores
  name: count
  type: integer
- description: Number of cores per CPU socket
  name: cores_per_socket
  type: integer
- description: Whether CPU hot-add is enabled
  name: hot_add_enabled
  type: boolean
- description: Whether CPU hot-remove is enabled
  name: hot_remove_enabled
  type: boolean
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-cpu-info-schema.json
slug: vmware-vsphere-cpu-info
source_filename: vmware-vsphere-cpu-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CpuInfo\",\n  \"type\": \"object\",\n  \"description\": \"CPU configuration of a virtual machine\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of virtual CPU cores\"\n    },\n    \"cores_per_socket\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of cores per CPU socket\"\n    },\n    \"hot_add_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether CPU hot-add is enabled\"\n    },\n    \"hot_remove_enabled\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether CPU hot-remove is enabled\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-cpu-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: CpuInfo
---
