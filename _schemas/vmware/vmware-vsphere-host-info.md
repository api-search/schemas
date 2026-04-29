---
description: Detailed ESXi host information
layout: schema
name: HostInfo
properties_list:
- description: Host name
  name: name
  type: string
- description: ''
  name: connection_state
  type: string
- description: ''
  name: power_state
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-host-info-schema.json
slug: vmware-vsphere-host-info
source_filename: vmware-vsphere-host-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostInfo\",\n  \"type\": \"object\",\n  \"description\": \"Detailed ESXi host information\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Host name\"\n    },\n    \"connection_state\": {\n      \"type\": \"string\"\n    },\n    \"power_state\": {\n      \"type\": \"string\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-host-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: HostInfo
---
