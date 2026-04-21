---
description: A CloudStack network resource providing connectivity for virtual machines.
layout: schema
name: Network
properties_list:
- description: UUID of the network.
  name: id
  type: string
- description: Display name of the network.
  name: name
  type: string
- description: Current state of the network.
  name: state
  type: string
- description: UUID of the zone containing the network.
  name: zoneid
  type: string
- description: Type of network (Isolated, Shared, L2).
  name: type
  type: string
- description: CIDR block of the network.
  name: cidr
  type: string
provider_name: Apache CloudStack
provider_slug: apache-cloudstack
schema_file: json-schema/cloudstack-api-network-schema.json
slug: cloudstack-api-network
tags:
- Apache
- Cloud
- IaaS
- Infrastructure
- Open Source
- Virtualization
title: Network
---
