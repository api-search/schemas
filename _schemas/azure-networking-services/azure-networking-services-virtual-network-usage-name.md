---
description: Usage strings container.
layout: schema
name: VirtualNetworkUsageName
properties_list:
- description: Localized subnet size and usage string.
  name: localizedValue
  type: string
- description: Subnet size and usage string.
  name: value
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-virtual-network-usage-name-schema.json
slug: azure-networking-services-virtual-network-usage-name
source_filename: azure-networking-services-virtual-network-usage-name-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-usage-name-schema.json\",\n  \"title\": \"VirtualNetworkUsageName\",\n  \"description\": \"Usage strings container.\",\n  \"properties\": {\n    \"localizedValue\": {\n      \"description\": \"Localized subnet size and usage string.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"Subnet size and usage string.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-usage-name-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkUsageName
---
