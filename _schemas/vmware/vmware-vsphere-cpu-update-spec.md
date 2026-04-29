---
description: Specification for CPU configuration
layout: schema
name: CpuUpdateSpec
properties_list:
- description: Number of virtual CPU cores
  name: count
  type: integer
- description: Number of cores per socket
  name: cores_per_socket
  type: integer
- description: ''
  name: hot_add_enabled
  type: boolean
- description: ''
  name: hot_remove_enabled
  type: boolean
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-cpu-update-spec-schema.json
slug: vmware-vsphere-cpu-update-spec
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"CpuUpdateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for CPU configuration\",\n  \"properties\": {\n    \"count\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of virtual CPU cores\"\n    },\n    \"cores_per_socket\": {\n      \"type\": \"integer\",\n      \"description\": \"Number of cores per socket\"\n    },\n    \"hot_add_enabled\": {\n      \"type\": \"boolean\"\n    },\n    \"hot_remove_enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-cpu-update-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: CpuUpdateSpec
---
