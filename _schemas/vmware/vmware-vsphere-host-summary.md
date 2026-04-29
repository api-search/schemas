---
description: Summary of an ESXi host in the vCenter inventory
layout: schema
name: HostSummary
properties_list:
- description: Unique identifier of the host (e.g., host-10)
  name: host
  type: string
- description: Display name or hostname of the ESXi host
  name: name
  type: string
- description: Connection state of the host
  name: connection_state
  type: string
- description: Power state of the host
  name: power_state
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-host-summary-schema.json
slug: vmware-vsphere-host-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"HostSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of an ESXi host in the vCenter inventory\",\n  \"properties\": {\n    \"host\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the host (e.g., host-10)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name or hostname of the ESXi host\"\n    },\n    \"connection_state\": {\n      \"type\": \"string\",\n      \"description\": \"Connection state of the host\"\n    },\n    \"power_state\": {\n      \"type\": \"string\",\n      \"description\": \"Power state of the host\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-host-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: HostSummary
---
