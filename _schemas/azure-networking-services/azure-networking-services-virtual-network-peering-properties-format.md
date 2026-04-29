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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-peering-properties-format-schema.json\",\n  \"title\": \"VirtualNetworkPeeringPropertiesFormat\",\n  \"description\": \"Properties of the virtual network peering.\",\n  \"properties\": {\n    \"allowForwardedTraffic\": {\n      \"description\": \"Whether the forwarded traffic from the VMs in the local virtual network will be allowed/disallowed in remote virtual network.\",\n      \"type\": \"boolean\"\n    },\n    \"allowGatewayTransit\": {\n      \"description\": \"If gateway links can be used in remote virtual networking to link to this virtual network.\",\n      \"type\": \"boolean\"\n    },\n    \"allowVirtualNetworkAccess\": {\n      \"description\": \"Whether the VMs in the local virtual network space would be able to access the VMs in remote virtual\
  \ network space.\",\n      \"type\": \"boolean\"\n    },\n    \"peeringState\": {\n      \"description\": \"The status of the virtual network peering.\",\n      \"enum\": [\n        \"Initiated\",\n        \"Connected\",\n        \"Disconnected\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"VirtualNetworkPeeringState\"\n      }\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    },\n    \"remoteAddressSpace\": {\n      \"$ref\": \"#/definitions/AddressSpace\",\n      \"description\": \"The reference of the remote virtual network address space.\"\n    },\n    \"remoteVirtualNetwork\": {\n\
  \      \"description\": \"Reference to another subresource.\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Resource ID.\",\n          \"type\": \"string\"\n        }\n      },\n      \"x-ms-azure-resource\": true\n    },\n    \"useRemoteGateways\": {\n      \"description\": \"If remote gateways can be used on this virtual network. If the flag is set to true, and allowGatewayTransit on remote peering is also true, virtual network will use gateways of remote virtual network for transit. Only one peering can have this flag set to true. This flag cannot be set if virtual network already has a gateway.\",\n      \"type\": \"boolean\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-peering-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkPeeringPropertiesFormat
---
