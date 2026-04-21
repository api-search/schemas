---
description: Properties of ServiceAssociationLink.
layout: schema
name: ServiceAssociationLinkPropertiesFormat
properties_list:
- description: If true, the resource can be deleted.
  name: allowDelete
  type: boolean
- description: Link to the external resource.
  name: link
  type: string
- description: Resource type of the linked resource.
  name: linkedResourceType
  type: string
- description: A list of locations.
  name: locations
  type: array
- description: The current provisioning state.
  name: provisioningState
  type: string
provider_name: Azure Networking Services
provider_slug: azure-networking-services
schema_file: json-schema/azure-networking-services-service-association-link-properties-format-schema.json
slug: azure-networking-services-service-association-link-properties-format
tags:
- Azure
- Cloud
- Infrastructure
- Microsoft
- Networking
title: ServiceAssociationLinkPropertiesFormat
---
