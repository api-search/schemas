---
description: Virtual Network resource.
layout: schema
name: VirtualNetwork
properties_list:
- description: A unique read-only string that changes whenever the resource is updated.
  name: etag
  type: string
- description: Properties of the virtual network.
  name: properties
  type: object
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-virtual-network-schema.json
slug: azure-networking-services-virtual-network
source_filename: azure-networking-services-virtual-network-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-schema.json\",\n  \"title\": \"VirtualNetwork\",\n  \"description\": \"Virtual Network resource.\",\n  \"properties\": {\n    \"etag\": {\n      \"description\": \"A unique read-only string that changes whenever the resource is updated.\",\n      \"type\": \"string\"\n    },\n    \"properties\": {\n      \"$ref\": \"#/definitions/VirtualNetworkPropertiesFormat\",\n      \"description\": \"Properties of the virtual network.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetwork
---
