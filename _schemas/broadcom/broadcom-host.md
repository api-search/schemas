---
description: A Host represents a physical ESXi server that provides compute, memory, storage, and networking resources to virtual machines within a vSphere or VCF environment.
layout: schema
name: Broadcom Host
properties_list:
- description: The unique identifier of the host.
  name: id
  type: string
- description: The hostname or display name of the host.
  name: name
  type: string
- description: The fully qualified domain name of the host.
  name: fqdn
  type: string
- description: The connection state of the host.
  name: connection_state
  type: string
- description: The power state of the host.
  name: power_state
  type: string
- description: The identifier of the cluster to which this host belongs.
  name: cluster
  type: string
- description: CPU resource information for the host.
  name: cpu
  type: object
- description: Memory resource information for the host.
  name: memory
  type: object
- description: The ESXi version running on the host.
  name: version
  type: string
- description: The commissioning status of the host in VCF.
  name: status
  type: string
- description: Network addresses assigned to the host.
  name: ip_addresses
  type: array
provider_name: Broadcom
provider_slug: broadcom
schema_file: json-schema/broadcom-host-schema.json
slug: broadcom-host
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
title: Broadcom Host
---
