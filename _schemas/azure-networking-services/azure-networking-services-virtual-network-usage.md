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
source_filename: azure-networking-services-virtual-network-usage-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-usage-schema.json\",\n  \"title\": \"VirtualNetworkUsage\",\n  \"description\": \"Usage details for subnet.\",\n  \"properties\": {\n    \"currentValue\": {\n      \"description\": \"Indicates number of IPs used from the Subnet.\",\n      \"format\": \"double\",\n      \"readOnly\": true,\n      \"type\": \"number\"\n    },\n    \"id\": {\n      \"description\": \"Subnet identifier.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"limit\": {\n      \"description\": \"Indicates the size of the subnet.\",\n      \"format\": \"double\",\n      \"readOnly\": true,\n      \"type\": \"number\"\n    },\n    \"name\": {\n      \"$ref\": \"#/definitions/VirtualNetworkUsageName\",\n      \"description\": \"The name containing common and\
  \ localized value for usage.\",\n      \"readOnly\": true\n    },\n    \"unit\": {\n      \"description\": \"Usage units. Returns 'Count'.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-usage-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkUsage
---
