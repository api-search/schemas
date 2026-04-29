---
description: Summary of a VM storage policy
layout: schema
name: StoragePolicySummary
properties_list:
- description: Identifier of the storage policy
  name: policy
  type: string
- description: Name of the storage policy
  name: name
  type: string
- description: Description of the storage policy
  name: description
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-storage-policy-summary-schema.json
slug: vmware-vsphere-storage-policy-summary
source_filename: vmware-vsphere-storage-policy-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StoragePolicySummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a VM storage policy\",\n  \"properties\": {\n    \"policy\": {\n      \"type\": \"string\",\n      \"description\": \"Identifier of the storage policy\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Name of the storage policy\"\n    },\n    \"description\": {\n      \"type\": \"string\",\n      \"description\": \"Description of the storage policy\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-storage-policy-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: StoragePolicySummary
---
