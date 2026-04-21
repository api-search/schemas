---
description: An update history of the ImmutabilityPolicy of a blob container.
layout: schema
name: UpdateHistoryProperty
properties_list:
- description: The immutability period for the blobs in the container since the policy creation, in days.
  name: immutabilityPeriodSinceCreationInDays
  type: integer
- description: Returns the Object ID of the user who updated the ImmutabilityPolicy.
  name: objectIdentifier
  type: string
- description: Returns the Tenant ID that issued the token for the user who updated the ImmutabilityPolicy.
  name: tenantId
  type: string
- description: Returns the date and time the ImmutabilityPolicy was updated.
  name: timestamp
  type: string
- description: 'The ImmutabilityPolicy update type of a blob container, possible values include: put, lock and extend.'
  name: update
  type: string
- description: Returns the User Principal Name of the user who updated the ImmutabilityPolicy.
  name: upn
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-update-history-property-schema.json
slug: azure-storage-account-update-history-property
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: UpdateHistoryProperty
---
