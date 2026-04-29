---
description: Specification for memory configuration
layout: schema
name: MemoryUpdateSpec
properties_list:
- description: Memory size in mebibytes
  name: size_MiB
  type: integer
- description: ''
  name: hot_add_enabled
  type: boolean
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-memory-update-spec-schema.json
slug: vmware-vsphere-memory-update-spec
source_filename: vmware-vsphere-memory-update-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"MemoryUpdateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for memory configuration\",\n  \"properties\": {\n    \"size_MiB\": {\n      \"type\": \"integer\",\n      \"description\": \"Memory size in mebibytes\"\n    },\n    \"hot_add_enabled\": {\n      \"type\": \"boolean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-memory-update-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: MemoryUpdateSpec
---
