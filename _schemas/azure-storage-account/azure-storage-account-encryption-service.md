---
description: A service that allows server-side encryption to be used.
layout: schema
name: EncryptionService
properties_list:
- description: A boolean indicating whether or not the service encrypts the data as it is stored.
  name: enabled
  type: boolean
- description: Encryption key type to be used for the encryption service. 'Account' key type implies that an account-scoped encryption key will be used. 'Service' key type implies that a default service key is used.
  name: keyType
  type: string
- description: Gets a rough estimate of the date/time when the encryption was last enabled by the user. Only returned when encryption is enabled. There might be some unencrypted blobs which were written after this t
  name: lastEnabledTime
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-encryption-service-schema.json
slug: azure-storage-account-encryption-service
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: EncryptionService
---
