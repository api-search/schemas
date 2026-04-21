---
description: The parameters to list SAS credentials of a storage account.
layout: schema
name: AccountSasParameters
properties_list:
- description: The key to sign the account SAS token with.
  name: keyToSign
  type: string
- description: The time at which the shared access signature becomes invalid.
  name: signedExpiry
  type: string
- description: An IP address or a range of IP addresses from which to accept requests.
  name: signedIp
  type: string
- description: 'The signed permissions for the account SAS. Possible values include: Read (r), Write (w), Delete (d), List (l), Add (a), Create (c), Update (u) and Process (p).'
  name: signedPermission
  type: string
- description: The protocol permitted for a request made with the account SAS.
  name: signedProtocol
  type: string
- description: 'The signed resource types that are accessible with the account SAS. Service (s): Access to service-level APIs; Container (c): Access to container-level APIs; Object (o): Access to object-level APIs fo'
  name: signedResourceTypes
  type: string
- description: 'The signed services accessible with the account SAS. Possible values include: Blob (b), Queue (q), Table (t), File (f).'
  name: signedServices
  type: string
- description: The time at which the SAS becomes valid.
  name: signedStart
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-account-sas-parameters-schema.json
slug: azure-storage-account-account-sas-parameters
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: AccountSasParameters
---
