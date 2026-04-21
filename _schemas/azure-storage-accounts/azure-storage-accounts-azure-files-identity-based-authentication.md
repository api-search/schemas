---
description: Settings for Azure Files identity based authentication.
layout: schema
name: AzureFilesIdentityBasedAuthentication
properties_list:
- description: Required if choose AD.
  name: activeDirectoryProperties
  type: object
- description: Indicates the directory service used.
  name: directoryServiceOptions
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-azure-files-identity-based-authentication-schema.json
slug: azure-storage-accounts-azure-files-identity-based-authentication
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: AzureFilesIdentityBasedAuthentication
---
