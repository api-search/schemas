---
description: Summary of a resource pool
layout: schema
name: ResourcePoolSummary
properties_list:
- description: Unique identifier of the resource pool
  name: resource_pool
  type: string
- description: Display name of the resource pool
  name: name
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-resource-pool-summary-schema.json
slug: vmware-vsphere-resource-pool-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ResourcePoolSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a resource pool\",\n  \"properties\": {\n    \"resource_pool\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the resource pool\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the resource pool\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-resource-pool-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: ResourcePoolSummary
---
