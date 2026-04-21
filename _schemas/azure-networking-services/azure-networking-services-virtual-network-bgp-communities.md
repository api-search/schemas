---
description: Bgp Communities sent over ExpressRoute with each route corresponding to a prefix in this VNET.
layout: schema
name: VirtualNetworkBgpCommunities
properties_list:
- description: The BGP community associated with the region of the virtual network
  name: regionalCommunity
  type: string
- description: The BGP community associated with the virtual network
  name: virtualNetworkCommunity
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-virtual-network-bgp-communities-schema.json
slug: azure-networking-services-virtual-network-bgp-communities
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkBgpCommunities
---
