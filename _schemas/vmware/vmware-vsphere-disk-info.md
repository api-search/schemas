---
description: Detailed virtual disk configuration
layout: schema
name: DiskInfo
properties_list:
- description: Display label of the virtual disk
  name: label
  type: string
- description: Type of host bus adapter
  name: type
  type: string
- description: Capacity of the virtual disk in bytes
  name: capacity
  type: integer
- description: Disk backing information
  name: backing
  type: object
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-disk-info-schema.json
slug: vmware-vsphere-disk-info
source_filename: vmware-vsphere-disk-info-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"DiskInfo\",\n  \"type\": \"object\",\n  \"description\": \"Detailed virtual disk configuration\",\n  \"properties\": {\n    \"label\": {\n      \"type\": \"string\",\n      \"description\": \"Display label of the virtual disk\"\n    },\n    \"type\": {\n      \"type\": \"string\",\n      \"description\": \"Type of host bus adapter\"\n    },\n    \"capacity\": {\n      \"type\": \"integer\",\n      \"description\": \"Capacity of the virtual disk in bytes\"\n    },\n    \"backing\": {\n      \"type\": \"object\",\n      \"description\": \"Disk backing information\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-disk-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: DiskInfo
---
