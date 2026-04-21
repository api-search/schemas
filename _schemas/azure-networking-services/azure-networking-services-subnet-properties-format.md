---
description: Properties of the subnet.
layout: schema
name: SubnetPropertiesFormat
properties_list:
- description: The address prefix for the subnet.
  name: addressPrefix
  type: string
- description: List of address prefixes for the subnet.
  name: addressPrefixes
  type: array
- description: An array of references to the delegations on the subnet.
  name: delegations
  type: array
- description: Array of IP configuration profiles which reference this subnet.
  name: ipConfigurationProfiles
  type: array
- description: An array of references to the network interface IP configurations using subnet.
  name: ipConfigurations
  type: array
- description: Reference to another subresource.
  name: natGateway
  type: object
- description: The reference of the NetworkSecurityGroup resource.
  name: networkSecurityGroup
  type: object
- description: Enable or Disable apply network policies on private end point in the subnet.
  name: privateEndpointNetworkPolicies
  type: string
- description: An array of references to private endpoints.
  name: privateEndpoints
  type: array
- description: Enable or Disable apply network policies on private link service in the subnet.
  name: privateLinkServiceNetworkPolicies
  type: string
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: A read-only string identifying the intention of use for this subnet based on delegations and other user-defined properties.
  name: purpose
  type: string
- description: An array of references to the external resources using subnet.
  name: resourceNavigationLinks
  type: array
- description: The reference of the RouteTable resource.
  name: routeTable
  type: object
- description: An array of references to services injecting into this subnet.
  name: serviceAssociationLinks
  type: array
- description: An array of service endpoint policies.
  name: serviceEndpointPolicies
  type: array
- description: An array of service endpoints.
  name: serviceEndpoints
  type: array
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-subnet-properties-format-schema.json
slug: azure-networking-services-subnet-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: SubnetPropertiesFormat
---
