---
description: Properties of the backend address pool.
layout: schema
name: BackendAddressPoolPropertiesFormat
properties_list:
- description: An array of references to IP addresses defined in network interfaces.
  name: backendIPConfigurations
  type: array
- description: An array of references to load balancing rules that use this backend address pool.
  name: loadBalancingRules
  type: array
- description: Reference to another subresource.
  name: outboundRule
  type: object
- description: An array of references to outbound rules that use this backend address pool.
  name: outboundRules
  type: array
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-backend-address-pool-properties-format-schema.json
slug: azure-networking-services-backend-address-pool-properties-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-backend-address-pool-properties-format-schema.json\",\n  \"title\": \"BackendAddressPoolPropertiesFormat\",\n  \"description\": \"Properties of the backend address pool.\",\n  \"properties\": {\n    \"backendIPConfigurations\": {\n      \"description\": \"An array of references to IP addresses defined in network interfaces.\",\n      \"items\": {\n        \"$ref\": \"./networkInterface.json#/definitions/NetworkInterfaceIPConfiguration\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"loadBalancingRules\": {\n      \"description\": \"An array of references to load balancing rules that use this backend address pool.\",\n      \"items\": {\n        \"description\": \"Reference to another subresource.\",\n        \"properties\": {\n       \
  \   \"id\": {\n            \"description\": \"Resource ID.\",\n            \"type\": \"string\"\n          }\n        },\n        \"x-ms-azure-resource\": true\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"outboundRule\": {\n      \"description\": \"Reference to another subresource.\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Resource ID.\",\n          \"type\": \"string\"\n        }\n      },\n      \"x-ms-azure-resource\": true\n    },\n    \"outboundRules\": {\n      \"description\": \"An array of references to outbound rules that use this backend address pool.\",\n      \"items\": {\n        \"description\": \"Reference to another subresource.\",\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Resource ID.\",\n            \"type\": \"string\"\n          }\n        },\n        \"x-ms-azure-resource\": true\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"provisioningState\"\
  : {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-backend-address-pool-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: BackendAddressPoolPropertiesFormat
---
