---
description: Summary of a virtual machine in the vCenter inventory
layout: schema
name: VMSummary
properties_list:
- description: Unique identifier of the virtual machine (e.g., vm-123)
  name: vm
  type: string
- description: Display name of the virtual machine
  name: name
  type: string
- description: Current power state of the VM
  name: power_state
  type: string
- description: Number of virtual CPUs
  name: cpu_count
  type: integer
- description: Memory size in mebibytes
  name: memory_size_MiB
  type: integer
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-vm-summary-schema.json
slug: vmware-vsphere-vm-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VMSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a virtual machine in the vCenter inventory\",\n  \"properties\": {\n    \"vm\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the virtual machine (e.g., vm-123)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the virtual machine\"\n    },\n    \"power_state\": {\n      \"type\": \"string\",\n      \"description\": \"Current power state of the VM\"\n    },\n    \"cpu_count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of virtual CPUs\"\n    },\n    \"memory_size_MiB\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory size in mebibytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-vm-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: VMSummary
---
