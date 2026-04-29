---
description: Details of NetworkIntentPolicyConfiguration for PrepareNetworkPoliciesRequest.
layout: schema
name: NetworkIntentPolicyConfiguration
properties_list:
- description: The name of the Network Intent Policy for storing in target subscription.
  name: networkIntentPolicyName
  type: string
- description: Source network intent policy.
  name: sourceNetworkIntentPolicy
  type: object
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-network-intent-policy-configuration-schema.json
slug: azure-networking-services-network-intent-policy-configuration
source_filename: azure-networking-services-network-intent-policy-configuration-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-network-intent-policy-configuration-schema.json\",\n  \"title\": \"NetworkIntentPolicyConfiguration\",\n  \"description\": \"Details of NetworkIntentPolicyConfiguration for PrepareNetworkPoliciesRequest.\",\n  \"properties\": {\n    \"networkIntentPolicyName\": {\n      \"description\": \"The name of the Network Intent Policy for storing in target subscription.\",\n      \"type\": \"string\"\n    },\n    \"sourceNetworkIntentPolicy\": {\n      \"$ref\": \"#/definitions/NetworkIntentPolicy\",\n      \"description\": \"Source network intent policy.\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-network-intent-policy-configuration-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: NetworkIntentPolicyConfiguration
---
