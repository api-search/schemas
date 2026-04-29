---
description: Summary of a virtual disk
layout: schema
name: DiskSummary
properties_list:
- description: Identifier of the virtual disk
  name: disk
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-disk-summary-schema.json
slug: vmware-vsphere-disk-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DiskSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a virtual disk\",\n  \"properties\": {\n    \"disk\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the virtual disk\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-disk-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: DiskSummary
---
