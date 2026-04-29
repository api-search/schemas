---
description: Specification for creating a new virtual machine
layout: schema
name: VMCreateSpec
properties_list:
- description: Display name for the new VM
  name: name
  type: string
- description: Guest operating system identifier
  name: guest_OS
  type: string
- description: Placement specification for the VM
  name: placement
  type: object
- description: Virtual hardware version
  name: hardware_version
  type: string
- description: Virtual disks to create with the VM
  name: disks
  type: array
- description: Network adapters to create with the VM
  name: nics
  type: array
- description: Boot configuration
  name: boot
  type: object
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-vm-create-spec-schema.json
slug: vmware-vsphere-vm-create-spec
source_filename: vmware-vsphere-vm-create-spec-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VMCreateSpec\",\n  \"type\": \"object\",\n  \"description\": \"Specification for creating a new virtual machine\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name for the new VM\"\n    },\n    \"guest_OS\": {\n      \"type\": \"string\",\n      \"description\": \"Guest operating system identifier\"\n    },\n    \"placement\": {\n      \"type\": \"object\",\n      \"description\": \"Placement specification for the VM\"\n    },\n    \"hardware_version\": {\n      \"type\": \"string\",\n      \"description\": \"Virtual hardware version\"\n    },\n    \"disks\": {\n      \"type\": \"array\",\n      \"description\": \"Virtual disks to create with the VM\"\n    },\n    \"nics\": {\n      \"type\": \"array\",\n      \"description\": \"Network adapters to create with the VM\"\n    },\n    \"boot\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Boot configuration\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-vm-create-spec-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: VMCreateSpec
---
