---
description: Detailed datacenter information
layout: schema
name: DatacenterInfo
properties_list:
- description: Display name of the datacenter
  name: name
  type: string
- description: Datastore folder identifier
  name: datastore_folder
  type: string
- description: Host folder identifier
  name: host_folder
  type: string
- description: Network folder identifier
  name: network_folder
  type: string
- description: VM folder identifier
  name: vm_folder
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-datacenter-info-schema.json
slug: vmware-vsphere-datacenter-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatacenterInfo\",\n  \"type\": \"object\",\n  \"description\": \"Detailed datacenter information\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the datacenter\"\n    },\n    \"datastore_folder\": {\n      \"type\": \"string\",\n      \"description\": \"Datastore folder identifier\"\n    },\n    \"host_folder\": {\n      \"type\": \"string\",\n      \"description\": \"Host folder identifier\"\n    },\n    \"network_folder\": {\n      \"type\": \"string\",\n      \"description\": \"Network folder identifier\"\n    },\n    \"vm_folder\": {\n      \"type\": \"string\",\n      \"description\": \"VM folder identifier\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-datacenter-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: DatacenterInfo
---
