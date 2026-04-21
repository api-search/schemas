---
description: Identity for the container group.
layout: schema
name: ContainerGroupIdentity
properties_list:
- description: The principal id of the container group identity. This property will only be provided for a system assigned identity.
  name: principalId
  type: string
- description: The tenant id associated with the container group. This property will only be provided for a system assigned identity.
  name: tenantId
  type: string
- description: The type of identity used for the container group. The type 'SystemAssigned, UserAssigned' includes both an implicitly created identity and a set of user assigned identities. The type 'None' will remo
  name: type
  type: string
- description: 'The list of user identities associated with the container group. The user identity dictionary key references will be ARM resource ids in the form: ''/subscriptions/{subscriptionId}/resourceGroups/{reso'
  name: userAssignedIdentities
  type: object
provider_name: Azure Container Instances
provider_slug: azure-container-instances
schema_file: json-schema/azure-container-instances-container-group-identity-schema.json
slug: azure-container-instances-container-group-identity
tags:
- Azure
- Cloud
- Container Instances
- Containers
- Microsoft
- Serverless
title: ContainerGroupIdentity
---
