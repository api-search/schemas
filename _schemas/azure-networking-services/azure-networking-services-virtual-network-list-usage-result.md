---
description: Response for the virtual networks GetUsage API service call.
layout: schema
name: VirtualNetworkListUsageResult
properties_list:
- description: The URL to get the next set of results.
  name: nextLink
  type: string
- description: VirtualNetwork usage stats.
  name: value
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-virtual-network-list-usage-result-schema.json
slug: azure-networking-services-virtual-network-list-usage-result
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-list-usage-result-schema.json\",\n  \"title\": \"VirtualNetworkListUsageResult\",\n  \"description\": \"Response for the virtual networks GetUsage API service call.\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URL to get the next set of results.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"VirtualNetwork usage stats.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/VirtualNetworkUsage\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-virtual-network-list-usage-result-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: VirtualNetworkListUsageResult
---
