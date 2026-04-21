---
description: A CloudStack virtual machine resource with its configuration and runtime state.
layout: schema
name: VirtualMachine
properties_list:
- description: UUID of the virtual machine.
  name: id
  type: string
- description: Display name of the virtual machine.
  name: name
  type: string
- description: Current state of the virtual machine.
  name: state
  type: string
- description: UUID of the zone containing the virtual machine.
  name: zoneid
  type: string
- description: Name of the zone containing the virtual machine.
  name: zonename
  type: string
- description: UUID of the service offering used by the virtual machine.
  name: serviceofferingid
  type: string
- description: UUID of the template used to create the virtual machine.
  name: templateid
  type: string
- description: Number of CPU cores.
  name: cpunumber
  type: integer
- description: Memory in megabytes.
  name: memory
  type: integer
- description: Primary IP address of the virtual machine.
  name: ipaddress
  type: string
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-virtual-machine-schema.json
slug: cloudstack-api-virtual-machine
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: VirtualMachine
---
