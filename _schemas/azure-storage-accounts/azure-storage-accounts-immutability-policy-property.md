---
description: The properties of an ImmutabilityPolicy of a blob container.
layout: schema
name: ImmutabilityPolicyProperty
properties_list:
- description: The immutability period for the blobs in the container since the policy creation, in days.
  name: immutabilityPeriodSinceCreationInDays
  type: integer
- description: 'The ImmutabilityPolicy state of a blob container, possible values include: Locked and Unlocked.'
  name: state
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-immutability-policy-property-schema.json
slug: azure-storage-accounts-immutability-policy-property
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ImmutabilityPolicyProperty
---
