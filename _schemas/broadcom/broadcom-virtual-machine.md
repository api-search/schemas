---
description: A Virtual Machine represents a software-based compute instance running on a vSphere host, with configurable CPU, memory, storage, and network resources.
layout: schema
name: Broadcom Virtual Machine
properties_list:
- description: The unique identifier of the virtual machine.
  name: vm
  type: string
- description: The display name of the virtual machine.
  name: name
  type: string
- description: The current power state of the virtual machine.
  name: power_state
  type: string
- description: The number of virtual CPUs allocated to the virtual machine.
  name: cpu_count
  type: integer
- description: The memory size in mebibytes allocated to the virtual machine.
  name: memory_size_MiB
  type: integer
- description: The guest operating system identifier.
  name: guest_OS
  type: string
- description: Hardware configuration of the virtual machine.
  name: hardware
  type: object
- description: The list of virtual disks attached to the virtual machine.
  name: disks
  type: array
- description: The list of virtual network interfaces.
  name: nics
  type: array
- description: Boot configuration for the virtual machine.
  name: boot
  type: object
- description: Tags associated with the virtual machine.
  name: tags
  type: array
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-virtual-machine-schema.json
slug: broadcom-virtual-machine
source_filename: broadcom-virtual-machine-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://github.com/api-evangelist/broadcom/blob/main/json-schema/broadcom-virtual-machine-schema.json\",\n  \"title\": \"Broadcom Virtual Machine\",\n  \"description\": \"A Virtual Machine represents a software-based compute instance running on a vSphere host, with configurable CPU, memory, storage, and network resources.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"vm\": {\n      \"type\": \"string\",\n      \"description\": \"The unique identifier of the virtual machine.\"\n    },\n    \"name\": {\n      \"type\": \"string\",\n      \"description\": \"The display name of the virtual machine.\"\n    },\n    \"power_state\": {\n      \"type\": \"string\",\n      \"enum\": [\n        \"POWERED_ON\",\n        \"POWERED_OFF\",\n        \"SUSPENDED\"\n      ],\n      \"description\": \"The current power state of the virtual machine.\"\n    },\n    \"cpu_count\": {\n      \"type\": \"integer\"\
  ,\n      \"description\": \"The number of virtual CPUs allocated to the virtual machine.\"\n    },\n    \"memory_size_MiB\": {\n      \"type\": \"integer\",\n      \"description\": \"The memory size in mebibytes allocated to the virtual machine.\"\n    },\n    \"guest_OS\": {\n      \"type\": \"string\",\n      \"description\": \"The guest operating system identifier.\"\n    },\n    \"hardware\": {\n      \"type\": \"object\",\n      \"description\": \"Hardware configuration of the virtual machine.\",\n      \"properties\": {\n        \"version\": {\n          \"type\": \"string\",\n          \"description\": \"The virtual hardware version.\"\n        },\n        \"upgrade_policy\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"NEVER\",\n            \"AFTER_CLEAN_SHUTDOWN\",\n            \"ALWAYS\"\n          ],\n          \"description\": \"The upgrade policy for virtual hardware.\"\n        }\n      }\n    },\n    \"disks\": {\n      \"type\": \"array\",\n\
  \      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The identifier of the virtual disk.\"\n          },\n          \"capacity\": {\n            \"type\": \"integer\",\n            \"description\": \"The capacity of the disk in bytes.\"\n          },\n          \"type\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"SCSI\",\n              \"SATA\",\n              \"IDE\",\n              \"NVME\"\n            ],\n            \"description\": \"The type of host bus adapter the disk is connected to.\"\n          }\n        }\n      },\n      \"description\": \"The list of virtual disks attached to the virtual machine.\"\n    },\n    \"nics\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"object\",\n        \"properties\": {\n          \"key\": {\n            \"type\": \"string\",\n            \"description\": \"The identifier\
  \ of the virtual NIC.\"\n          },\n          \"mac_address\": {\n            \"type\": \"string\",\n            \"description\": \"The MAC address of the NIC.\"\n          },\n          \"backing_type\": {\n            \"type\": \"string\",\n            \"description\": \"The backing type for the virtual NIC.\"\n          },\n          \"state\": {\n            \"type\": \"string\",\n            \"enum\": [\n              \"CONNECTED\",\n              \"NOT_CONNECTED\"\n            ],\n            \"description\": \"The connection state of the NIC.\"\n          }\n        }\n      },\n      \"description\": \"The list of virtual network interfaces.\"\n    },\n    \"boot\": {\n      \"type\": \"object\",\n      \"description\": \"Boot configuration for the virtual machine.\",\n      \"properties\": {\n        \"type\": {\n          \"type\": \"string\",\n          \"enum\": [\n            \"BIOS\",\n            \"EFI\"\n          ],\n          \"description\": \"The firmware type used\
  \ for booting.\"\n        },\n        \"delay\": {\n          \"type\": \"integer\",\n          \"description\": \"Boot delay in milliseconds.\"\n        }\n      }\n    },\n    \"tags\": {\n      \"type\": \"array\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"description\": \"Tags associated with the virtual machine.\"\n    }\n  }\n}\n"
source_json_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/json-schema/broadcom-virtual-machine-schema.json
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Virtual Machine
---
