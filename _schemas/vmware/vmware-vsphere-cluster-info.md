---
description: Detailed cluster configuration
layout: schema
name: ClusterInfo
properties_list:
- description: Display name of the cluster
  name: name
  type: string
- description: Root resource pool of the cluster
  name: resource_pool
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-cluster-info-schema.json
slug: vmware-vsphere-cluster-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ClusterInfo\",\n  \"type\": \"object\",\n  \"description\": \"Detailed cluster configuration\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the cluster\"\n    },\n    \"resource_pool\": {\n      \"type\": \"string\",\n      \"description\": \"Root resource pool of the cluster\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-cluster-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: ClusterInfo
---
