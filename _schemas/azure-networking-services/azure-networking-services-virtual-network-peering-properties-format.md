---
description: Properties of the virtual network peering.
layout: schema
name: VirtualNetworkPeeringPropertiesFormat
properties_list:
- description: Whether the forwarded traffic from the VMs in the local virtual network will be allowed/disallowed in remote virtual network.
  name: allowForwardedTraffic
  type: boolean
- description: If gateway links can be used in remote virtual networking to link to this virtual network.
  name: allowGatewayTransit
  type: boolean
- description: Whether the VMs in the local virtual network space would be able to access the VMs in remote virtual network space.
  name: allowVirtualNetworkAccess
  type: boolean
- description: The status of the virtual network peering.
  name: peeringState
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The reference of the remote virtual network address space.
  name: remoteAddressSpace
  type: object
- description: Reference to another subresource.
  name: remoteVirtualNetwork
  type: object
- description: 'If remote gateways can be used on this virtual network. If the flag is set to true, and allowGatewayTransit on remote peering is also true, virtual network will use gateways of remote virtual network '
  name: useRemoteGateways
  type: boolean
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-virtual-network-peering-properties-format-schema.json
slug: azure-networking-services-virtual-network-peering-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkPeeringPropertiesFormat
---
