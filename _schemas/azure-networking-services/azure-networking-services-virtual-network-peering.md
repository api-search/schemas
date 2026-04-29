---
description: Peerings in a virtual network resource.
layout: schema
name: VirtualNetworkPeering
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: The name of the resource that is unique within a resource group. This name can be used to access the resource.
  name: name
  type: string
- description: Properties of the virtual network peering.
  name: properties
  type: object
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-virtual-network-peering-schema.json
slug: azure-networking-services-virtual-network-peering
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-peering-schema.json\",\n  \"title\": \"VirtualNetworkPeering\",\n  \"description\": \"Peerings in a virtual network resource.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n      \"type\": \"string\"\n    },\n    \"name\": {\n      \"description\": \"The name of the resource that is unique within a resource group. This name can be used to access the resource.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/VirtualNetworkPeeringPropertiesFormat\",\n      \"description\": \"Properties of the virtual network peering.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-peering-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkPeering
---
