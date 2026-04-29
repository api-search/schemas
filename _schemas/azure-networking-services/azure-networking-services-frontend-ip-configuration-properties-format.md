---
description: Properties of Frontend IP Configuration of the load balancer.
layout: schema
name: FrontendIPConfigurationPropertiesFormat
properties_list:
- description: An array of references to inbound pools that use this frontend IP.
  name: inboundNatPools
  type: array
- description: An array of references to inbound rules that use this frontend IP.
  name: inboundNatRules
  type: array
- description: An array of references to load balancing rules that use this frontend IP.
  name: loadBalancingRules
  type: array
- description: An array of references to outbound rules that use this frontend IP.
  name: outboundRules
  type: array
- description: The private IP address of the IP configuration.
  name: privateIPAddress
  type: string
- description: IP address version.
  name: privateIPAddressVersion
  type: string
- description: IP address allocation method.
  name: privateIPAllocationMethod
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The reference of the Public IP resource.
  name: publicIPAddress
  type: object
- description: Reference to another subresource.
  name: publicIPPrefix
  type: object
- description: The reference of the subnet resource.
  name: subnet
  type: object
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-frontend-ip-configuration-properties-format-schema.json
slug: azure-networking-services-frontend-ip-configuration-properties-format
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-frontend-ip-configuration-properties-format-schema.json\",\n  \"title\": \"FrontendIPConfigurationPropertiesFormat\",\n  \"description\": \"Properties of Frontend IP Configuration of the load balancer.\",\n  \"properties\": {\n    \"inboundNatPools\": {\n      \"description\": \"An array of references to inbound pools that use this frontend IP.\",\n      \"items\": {\n        \"description\": \"Reference to another subresource.\",\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Resource ID.\",\n            \"type\": \"string\"\n          }\n        },\n        \"x-ms-azure-resource\": true\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"inboundNatRules\": {\n      \"description\": \"An array of references\
  \ to inbound rules that use this frontend IP.\",\n      \"items\": {\n        \"description\": \"Reference to another subresource.\",\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Resource ID.\",\n            \"type\": \"string\"\n          }\n        },\n        \"x-ms-azure-resource\": true\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"loadBalancingRules\": {\n      \"description\": \"An array of references to load balancing rules that use this frontend IP.\",\n      \"items\": {\n        \"description\": \"Reference to another subresource.\",\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Resource ID.\",\n            \"type\": \"string\"\n          }\n        },\n        \"x-ms-azure-resource\": true\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"outboundRules\": {\n      \"description\": \"An array of references to outbound rules that use this frontend\
  \ IP.\",\n      \"items\": {\n        \"description\": \"Reference to another subresource.\",\n        \"properties\": {\n          \"id\": {\n            \"description\": \"Resource ID.\",\n            \"type\": \"string\"\n          }\n        },\n        \"x-ms-azure-resource\": true\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    },\n    \"privateIPAddress\": {\n      \"description\": \"The private IP address of the IP configuration.\",\n      \"type\": \"string\"\n    },\n    \"privateIPAddressVersion\": {\n      \"description\": \"IP address version.\",\n      \"enum\": [\n        \"IPv4\",\n        \"IPv6\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"IPVersion\"\n      }\n    },\n    \"privateIPAllocationMethod\": {\n      \"description\": \"IP address allocation method.\",\n      \"enum\": [\n        \"Static\",\n        \"Dynamic\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\"\
  : {\n        \"modelAsString\": true,\n        \"name\": \"IPAllocationMethod\"\n      }\n    },\n    \"provisioningState\": {\n      \"description\": \"The current provisioning state.\",\n      \"enum\": [\n        \"Succeeded\",\n        \"Updating\",\n        \"Deleting\",\n        \"Failed\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"ProvisioningState\"\n      }\n    },\n    \"publicIPAddress\": {\n      \"$ref\": \"./publicIpAddress.json#/definitions/PublicIPAddress\",\n      \"description\": \"The reference of the Public IP resource.\"\n    },\n    \"publicIPPrefix\": {\n      \"description\": \"Reference to another subresource.\",\n      \"properties\": {\n        \"id\": {\n          \"description\": \"Resource ID.\",\n          \"type\": \"string\"\n        }\n      },\n      \"x-ms-azure-resource\": true\n    },\n    \"subnet\": {\n      \"$ref\": \"./virtualNetwork.json#/definitions/Subnet\"\
  ,\n      \"description\": \"The reference of the subnet resource.\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-networking-services/refs/heads/main/json-schema/azure-networking-services-frontend-ip-configuration-properties-format-schema.json
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: FrontendIPConfigurationPropertiesFormat
---
