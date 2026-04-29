---
description: Guest OS networking information from VMware Tools
layout: schema
name: GuestNetworkingInfo
properties_list:
- description: ''
  name: dns_values
  type: object
- description: ''
  name: dns
  type: object
- description: ''
  name: interfaces
  type: array
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-guest-networking-info-schema.json
slug: vmware-vsphere-guest-networking-info
source_filename: vmware-vsphere-guest-networking-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"GuestNetworkingInfo\",\n  \"type\": \"object\",\n  \"description\": \"Guest OS networking information from VMware Tools\",\n  \"properties\": {\n    \"dns_values\": {\n      \"type\": \"object\"\n    },\n    \"dns\": {\n      \"type\": \"object\"\n    },\n    \"interfaces\": {\n      \"type\": \"array\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-guest-networking-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: GuestNetworkingInfo
---
