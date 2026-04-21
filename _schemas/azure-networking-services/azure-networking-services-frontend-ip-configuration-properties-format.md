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
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: FrontendIPConfigurationPropertiesFormat
---
