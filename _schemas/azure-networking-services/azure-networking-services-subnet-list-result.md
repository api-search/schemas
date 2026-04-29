---
description: Response for ListSubnets API service callRetrieves all subnet that belongs to a virtual network.
layout: schema
name: SubnetListResult
properties_list:
- description: The URL to get the next set of results.
  name: nextLink
  type: string
- description: The subnets in a virtual network.
  name: value
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-subnet-list-result-schema.json
slug: azure-networking-services-subnet-list-result
source_filename: azure-networking-services-subnet-list-result-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-subnet-list-result-schema.json\",\n  \"title\": \"SubnetListResult\",\n  \"description\": \"Response for ListSubnets API service callRetrieves all subnet that belongs to a virtual network.\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"The URL to get the next set of results.\",\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"The subnets in a virtual network.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/Subnet\"\n      },\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-subnet-list-result-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: SubnetListResult
---
