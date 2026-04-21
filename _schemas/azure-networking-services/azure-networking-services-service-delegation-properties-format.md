---
description: Properties of a service delegation.
layout: schema
name: ServiceDelegationPropertiesFormat
properties_list:
- description: Describes the actions permitted to the service upon delegation.
  name: actions
  type: array
- description: The current provisioning state.
  name: provisioningState
  type: string
- description: The name of the service to whom the subnet should be delegated (e.g. Microsoft.Sql/servers).
  name: serviceName
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-service-delegation-properties-format-schema.json
slug: azure-networking-services-service-delegation-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ServiceDelegationPropertiesFormat
---
