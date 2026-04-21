---
description: The properties of a container.
layout: schema
name: ContainerProperties
properties_list:
- description: The hasImmutabilityPolicy public property is set to true by SRP if ImmutabilityPolicy has been created for this container. The hasImmutabilityPolicy public property is set to false by SRP if Immutabil
  name: hasImmutabilityPolicy
  type: boolean
- description: 'The hasLegalHold public property is set to true by SRP if there are at least one existing tag. The hasLegalHold public property is set to false by SRP if all existing legal hold tags are cleared out. '
  name: hasLegalHold
  type: boolean
- description: The ImmutabilityPolicy property of the container.
  name: immutabilityPolicy
  type: object
- description: Returns the date and time the container was last modified.
  name: lastModifiedTime
  type: string
- description: Specifies whether the lease on a container is of infinite or fixed duration, only when the container is leased.
  name: leaseDuration
  type: string
- description: Lease state of the container.
  name: leaseState
  type: string
- description: The lease status of the container.
  name: leaseStatus
  type: string
- description: The LegalHold property of the container.
  name: legalHold
  type: object
- description: A name-value pair to associate with the container as metadata.
  name: metadata
  type: object
- description: Specifies whether data in the container may be accessed publicly and the level of access.
  name: publicAccess
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-container-properties-schema.json
slug: azure-storage-accounts-container-properties
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ContainerProperties
---
