---
description: Properties of the virtual network.
layout: schema
name: VirtualNetworkPropertiesFormat
properties_list:
- description: The AddressSpace that contains an array of IP address ranges that can be used by subnets.
  name: addressSpace
  type: object
- description: Bgp Communities sent over ExpressRoute with each route corresponding to a prefix in this VNET.
  name: bgpCommunities
  type: object
- description: Reference to another subresource.
  name: ddosProtectionPlan
  type: object
- description: The dhcpOptions that contains an array of DNS servers available to VMs deployed in the virtual network.
  name: dhcpOptions
  type: object
- description: Indicates if DDoS protection is enabled for all the protected resources in the virtual network. It requires a DDoS protection plan associated with the resource.
  name: enableDdosProtection
  type: boolean
- description: Indicates if VM protection is enabled for all the subnets in the virtual network.
  name: enableVmProtection
  type: boolean
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The resourceGuid property of the Virtual Network resource.
  name: resourceGuid
  type: string
- description: A list of subnets in a Virtual Network.
  name: subnets
  type: array
- description: A list of peerings in a Virtual Network.
  name: virtualNetworkPeerings
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-virtual-network-properties-format-schema.json
slug: azure-networking-services-virtual-network-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkPropertiesFormat
---
