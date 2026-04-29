---
description: Power state information for a virtual machine
layout: schema
name: PowerInfo
properties_list:
- description: Current power state
  name: state
  type: string
- description: Whether the last power-off was clean
  name: clean_power_off
  type: boolean
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-power-info-schema.json
slug: vmware-vsphere-power-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"PowerInfo\",\n  \"type\": \"object\",\n  \"description\": \"Power state information for a virtual machine\",\n  \"properties\": {\n    \"state\": {\n      \"type\": \"string\",\n      \"description\": \"Current power state\"\n    },\n    \"clean_power_off\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the last power-off was clean\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-power-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: PowerInfo
---
