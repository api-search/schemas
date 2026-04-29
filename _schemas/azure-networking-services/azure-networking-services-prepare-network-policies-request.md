---
description: Details of PrepareNetworkPolicies for Subnet.
layout: schema
name: PrepareNetworkPoliciesRequest
properties_list:
- description: A list of NetworkIntentPolicyConfiguration.
  name: networkIntentPolicyConfigurations
  type: array
- description: The name of the service for which subnet is being prepared for.
  name: serviceName
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-prepare-network-policies-request-schema.json
slug: azure-networking-services-prepare-network-policies-request
source_filename: azure-networking-services-prepare-network-policies-request-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-prepare-network-policies-request-schema.json\",\n  \"title\": \"PrepareNetworkPoliciesRequest\",\n  \"description\": \"Details of PrepareNetworkPolicies for Subnet.\",\n  \"properties\": {\n    \"networkIntentPolicyConfigurations\": {\n      \"description\": \"A list of NetworkIntentPolicyConfiguration.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/NetworkIntentPolicyConfiguration\"\n      },\n      \"type\": \"array\"\n    },\n    \"serviceName\": {\n      \"description\": \"The name of the service for which subnet is being prepared for.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-prepare-network-policies-request-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: PrepareNetworkPoliciesRequest
---
