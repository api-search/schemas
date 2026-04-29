---
description: DhcpOptions contains an array of DNS servers available to VMs deployed in the virtual network. Standard DHCP option for a subnet overrides VNET DHCP options.
layout: schema
name: DhcpOptions
properties_list:
- description: The list of DNS servers IP addresses.
  name: dnsServers
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-dhcp-options-schema.json
slug: azure-networking-services-dhcp-options
source_filename: azure-networking-services-dhcp-options-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-dhcp-options-schema.json\",\n  \"title\": \"DhcpOptions\",\n  \"description\": \"DhcpOptions contains an array of DNS servers available to VMs deployed in the virtual network. Standard DHCP option for a subnet overrides VNET DHCP options.\",\n  \"properties\": {\n    \"dnsServers\": {\n      \"description\": \"The list of DNS servers IP addresses.\",\n      \"items\": {\n        \"type\": \"string\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-dhcp-options-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: DhcpOptions
---
