---
description: The encryption settings on the storage account.
layout: schema
name: Encryption
properties_list:
- description: 'The encryption keySource (provider). Possible values (case-insensitive): Microsoft.Storage, Microsoft.Keyvault'
  name: keySource
  type: string
- description: Properties provided by key vault.
  name: keyvaultproperties
  type: object
- description: List of services which support encryption.
  name: services
  type: object
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-encryption-schema.json
slug: azure-storage-accounts-encryption
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: Encryption
---
