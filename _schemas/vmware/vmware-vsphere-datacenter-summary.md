---
description: Summary of a datacenter
layout: schema
name: DatacenterSummary
properties_list:
- description: Unique identifier of the datacenter
  name: datacenter
  type: string
- description: Display name of the datacenter
  name: name
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-datacenter-summary-schema.json
slug: vmware-vsphere-datacenter-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatacenterSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a datacenter\",\n  \"properties\": {\n    \"datacenter\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the datacenter\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the datacenter\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-datacenter-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: DatacenterSummary
---
