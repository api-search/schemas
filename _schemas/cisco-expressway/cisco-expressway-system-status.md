---
description: Schema for the system status overview of a Cisco Expressway node. Includes system identification, software and hardware versions, network configuration, resource usage, cluster role, and option key status.
layout: schema
name: Cisco Expressway System Status
properties_list:
- description: The name assigned to the Expressway node
  name: SystemName
  type: string
- description: Currently installed software version
  name: SoftwareVersion
  type: string
- description: Hardware appliance version or VM designation
  name: HardwareVersion
  type: string
- description: Hardware or VM serial number used for identification and licensing
  name: SerialNumber
  type: string
- description: Time elapsed since the system last restarted, in human-readable format
  name: Uptime
  type: string
- description: IPv4 address of the Expressway node
  name: IPv4Address
  type: string
- description: IPv6 address of the Expressway node, if configured
  name: IPv6Address
  type:
  - string
  - 'null'
- description: Virtual machine size designation which determines capacity limits
  name: VMSize
  type: string
- description: Number of devices currently registered with this Expressway node
  name: CurrentRegistrations
  type: integer
- description: Number of calls currently active on this Expressway node
  name: CurrentCalls
  type: integer
- description: Role of this node in a cluster configuration
  name: ClusterRole
  type: string
- description: List of installed option keys and their activation status
  name: OptionKeys
  type: array
provider_name: Cisco Expressway
provider_slug: cisco-expressway
schema_file: json-schema/cisco-expressway-system-status-schema.json
slug: cisco-expressway-system-status
tags:
- Collaboration
- Firewall Traversal
- H.323
- Session Border Controller
- SIP
- Unified Communications
- Video Conferencing
title: Cisco Expressway System Status
---
