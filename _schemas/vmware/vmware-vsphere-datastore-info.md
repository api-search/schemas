---
description: Detailed datastore configuration and status
layout: schema
name: DatastoreInfo
properties_list:
- description: Display name of the datastore
  name: name
  type: string
- description: ''
  name: type
  type: string
- description: Whether the datastore is currently accessible
  name: accessible
  type: boolean
- description: Available free space in bytes
  name: free_space
  type: integer
- description: Maximum capacity in bytes
  name: capacity
  type: integer
- description: Whether thin provisioning is supported
  name: thin_provisioning_supported
  type: boolean
- description: Whether the datastore is accessible by multiple hosts
  name: multiple_host_access
  type: boolean
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-datastore-info-schema.json
slug: vmware-vsphere-datastore-info
source_filename: vmware-vsphere-datastore-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DatastoreInfo\",\n  \"type\": \"object\",\n  \"description\": \"Detailed datastore configuration and status\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the datastore\"\n    },\n    \"type\": {\n      \"type\": \"string\"\n    },\n    \"accessible\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the datastore is currently accessible\"\n    },\n    \"free_space\": {\n      \"type\": \"integer\",\n      \"description\": \"Available free space in bytes\"\n    },\n    \"capacity\": {\n      \"type\": \"integer\",\n      \"description\": \"Maximum capacity in bytes\"\n    },\n    \"thin_provisioning_supported\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether thin provisioning is supported\"\n    },\n    \"multiple_host_access\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether\
  \ the datastore is accessible by multiple hosts\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-datastore-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: DatastoreInfo
---
