---
description: Summary of a virtual network adapter
layout: schema
name: EthernetSummary
properties_list:
- description: Identifier of the network adapter
  name: nic
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-ethernet-summary-schema.json
slug: vmware-vsphere-ethernet-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"EthernetSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a virtual network adapter\",\n  \"properties\": {\n    \"nic\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the network adapter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-ethernet-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: EthernetSummary
---
