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
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: BackendAddressPoolPropertiesFormat
---
