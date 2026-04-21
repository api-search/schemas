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
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Virtual Machine
---
