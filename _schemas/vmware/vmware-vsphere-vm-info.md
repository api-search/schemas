---
description: Detailed virtual machine configuration and state
layout: schema
name: VMInfo
properties_list:
- description: Display name of the virtual machine
  name: name
  type: string
- description: VM identity information
  name: identity
  type: object
- description: ''
  name: power_state
  type: string
- description: Configured guest operating system
  name: guest_OS
  type: string
- description: ''
  name: boot
  type: object
- description: Map of disk identifier to disk configuration
  name: disks
  type: object
- description: Map of NIC identifier to NIC configuration
  name: nics
  type: object
- description: Map of CD-ROM identifier to CD-ROM configuration
  name: cdroms
  type: object
- description: ''
  name: parallel_ports
  type: object
- description: ''
  name: serial_ports
  type: object
- description: ''
  name: floppy_drives
  type: object
provider_name: VMware
provider_slug: vmware
schema_file: json-schema/vmware-vsphere-vm-info-schema.json
slug: vmware-vsphere-vm-info
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"VMInfo\",\n  \"type\": \"object\",\n  \"description\": \"Detailed virtual machine configuration and state\",\n  \"properties\": {\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"Display name of the virtual machine\"\n    },\n    \"identity\": {\n      \"type\": \"object\",\n      \"description\": \"VM identity information\"\n    },\n    \"power_state\": {\n      \"type\": \"string\"\n    },\n    \"guest_OS\": {\n      \"type\": \"string\",\n      \"description\": \"Configured guest operating system\"\n    },\n    \"boot\": {\n      \"type\": \"object\"\n    },\n    \"disks\": {\n      \"type\": \"object\",\n      \"description\": \"Map of disk identifier to disk configuration\"\n    },\n    \"nics\": {\n      \"type\": \"object\",\n      \"description\": \"Map of NIC identifier to NIC configuration\"\n    },\n    \"cdroms\": {\n      \"type\": \"object\",\n      \"description\"\
  : \"Map of CD-ROM identifier to CD-ROM configuration\"\n    },\n    \"parallel_ports\": {\n      \"type\": \"object\"\n    },\n    \"serial_ports\": {\n      \"type\": \"object\"\n    },\n    \"floppy_drives\": {\n      \"type\": \"object\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/json-schema/vmware-vsphere-vm-info-schema.json
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
title: VMInfo
---
