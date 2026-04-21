---
description: Usage details for subnet.
layout: schema
name: VirtualNetworkUsage
properties_list:
- description: Indicates number of IPs used from the Subnet.
  name: currentValue
  type: number
- description: Subnet identifier.
  name: id
  type: string
- description: Indicates the size of the subnet.
  name: limit
  type: number
- description: The name containing common and localized value for usage.
  name: name
  type: object
- description: Usage units. Returns 'Count'.
  name: unit
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-virtual-network-usage-schema.json
slug: azure-networking-services-virtual-network-usage
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkUsage
---
