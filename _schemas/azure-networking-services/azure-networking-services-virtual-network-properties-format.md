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
source_filename: azure-networking-services-virtual-network-properties-format-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-properties-format-schema.json\",\n  \"title\": \"VirtualNetworkPropertiesFormat\",\n  \"description\": \"Properties of the virtual network.\",\n  \"properties\": {\n    \"addressSpace\": {\n      \"$ref\": \"#/definitions/AddressSpace\",\n      \"description\": \"The AddressSpace that contains an array of IP address ranges that can be used by subnets.\"\n    },\n    \"bgpCommunities\": {\n      \"$ref\": \"#/definitions/VirtualNetworkBgpCommunities\",\n      \"description\": \"Bgp Communities sent over ExpressRoute with each route corresponding to a prefix in this VNET.\"\n    },\n    \"ddosProtectionPlan\": {\n      \"description\": \"Reference to another subresource.\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Resource\
  \ ID.\",\n          \"type\": \"string\"\n        }\n      },\n      \"x-ms-azure-resource\": true\n    },\n    \"dhcpOptions\": {\n      \"$ref\": \"#/definitions/DhcpOptions\",\n      \"description\": \"The dhcpOptions that contains an array of DNS servers available to VMs deployed in the virtual network.\"\n    },\n    \"enableDdosProtection\": {\n      \"default\": false,\n      \"description\": \"Indicates if DDoS protection is enabled for all the protected resources in the virtual network. It requires a DDoS protection plan associated with the resource.\",\n      \"type\": \"boolean\"\n    },\n    \"enableVmProtection\": {\n      \"default\": false,\n      \"description\": \"Indicates if VM protection is enabled for all the subnets in the virtual network.\",\n      \"type\": \"boolean\"\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n      \
  \  \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    },\n    \"resourceGuid\": {\n      \"description\": \"The resourceGuid property of the Virtual Network resource.\",\n      \"type\": \"string\"\n    },\n    \"subnets\": {\n      \"description\": \"A list of subnets in a Virtual Network.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Subnet\"\n      },\n      \"type\": \"array\"\n    },\n    \"virtualNetworkPeerings\": {\n      \"description\": \"A list of peerings in a Virtual Network.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/VirtualNetworkPeering\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkPropertiesFormat
---
