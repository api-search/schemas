---
description: Managed identity for the resource.
layout: schema
name: IdentityProperties
properties_list:
- description: The principal ID of resource identity.
  name: principalId
  type: string
- description: The tenant ID of resource.
  name: tenantId
  type: string
- description: The identity type.
  name: type
  type: string
- description: 'The list of user identities associated with the resource. The user identity dictionary key references will be ARM resource ids in the form: ''/subscriptions/{subscriptionId}/resourceGroups/{resourceGro'
  name: userAssignedIdentities
  type: object
provider_name: Azure Container Registry
provider_slug: azure-container-registry
schema_file: json-schema/azure-container-registry-identity-properties-schema.json
slug: azure-container-registry-identity-properties
tags:
- Azure
- Container Images
- Containers
- Docker
- Registry
title: IdentityProperties
---
