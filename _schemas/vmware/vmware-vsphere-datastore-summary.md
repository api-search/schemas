---
description: Summary of a datastore in the vCenter inventory
layout: schema
name: DatastoreSummary
properties_list:
- description: Unique identifier of the datastore (e.g., datastore-15)
  name: datastore
  type: string
- description: Display name of the datastore
  name: name
  type: string
- description: Type of the datastore
  name: type
  type: string
- description: Free space in bytes
  name: free_space
  type: integer
- description: Total capacity in bytes
  name: capacity
  type: integer
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-datastore-summary-schema.json
slug: vmware-vsphere-datastore-summary
source_filename: vmware-vsphere-datastore-summary-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatastoreSummary\",\n  \"type\": \"object\",\n  \"description\": \"Summary of a datastore in the vCenter inventory\",\n  \"properties\": {\n    \"datastore\": {\n      \"type\": \"string\",\n      \"description\": \"Unique identifier of the datastore (e.g., datastore-15)\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the datastore\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of the datastore\"\n    },\n    \"free_space\": {\n      \"type\": \"integer\",\n      \"description\": \"Free space in bytes\"\n    },\n    \"capacity\": {\n      \"type\": \"integer\",\n      \"description\": \"Total capacity in bytes\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-datastore-summary-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: DatastoreSummary
---
