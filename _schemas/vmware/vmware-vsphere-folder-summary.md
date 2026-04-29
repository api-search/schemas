---
description: Summary of an inventory folder
layout: schema
name: FolderSummary
properties_list:
- description: Unique identifier of the folder
  name: folder
  type: string
- description: Display name of the folder
  name: name
  type: string
- description: Type of folder
  name: type
  type: string
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-folder-summary-schema.json
slug: vmware-vsphere-folder-summary
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"FolderSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of an inventory folder\",\n  \"properties\": {\n    \"folder\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the folder\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the folder\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of folder\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-folder-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: FolderSummary
---
