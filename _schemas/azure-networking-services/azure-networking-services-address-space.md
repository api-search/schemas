---
description: AddressSpace contains an array of IP address ranges that can be used by subnets of the virtual network.
layout: schema
name: AddressSpace
properties_list:
- description: A list of address blocks reserved for this virtual network in CIDR notation.
  name: addressPrefixes
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-address-space-schema.json
slug: azure-networking-services-address-space
source_filename: azure-networking-services-address-space-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-address-space-schema.json\",\n  \"title\": \"AddressSpace\",\n  \"description\": \"AddressSpace contains an array of IP address ranges that can be used by subnets of the virtual network.\",\n  \"properties\": {\n    \"addressPrefixes\": {\n      \"description\": \"A list of address blocks reserved for this virtual network in CIDR notation.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-address-space-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: AddressSpace
---
