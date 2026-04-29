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
source_filename: azure-networking-services-virtual-network-bgp-communities-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-bgp-communities-schema.json\",\n  \"title\": \"VirtualNetworkBgpCommunities\",\n  \"description\": \"Bgp Communities sent over ExpressRoute with each route corresponding to a prefix in this VNET.\",\n  \"properties\": {\n    \"regionalCommunity\": {\n      \"description\": \"The BGP community associated with the region of the virtual network\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"virtualNetworkCommunity\": {\n      \"description\": \"The BGP community associated with the virtual network\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"virtualNetworkCommunity\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-bgp-communities-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkBgpCommunities
---
