---
description: Summary of a network in the vCenter inventory
layout: schema
name: NetworkSummary
properties_list:
- description: Unique identifier of the network
  name: network
  type: string
- description: Display name of the network
  name: name
  type: string
- description: Type of the network
  name: type
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-network-summary-schema.json
slug: vmware-vsphere-network-summary
source_filename: vmware-vsphere-network-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"NetworkSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a network in the vCenter inventory\",\n  \"properties\": {\n    \"network\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the network\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the network\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the network\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-network-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: NetworkSummary
---
