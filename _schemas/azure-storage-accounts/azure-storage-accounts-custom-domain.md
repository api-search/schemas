---
description: The custom domain assigned to this storage account. This can be set via Update.
layout: schema
name: CustomDomain
properties_list:
- description: Gets or sets the custom domain name assigned to the storage account. Name is the CNAME source.
  name: name
  type: string
- description: Indicates whether indirect CName validation is enabled. Default value is false. This should only be set on updates.
  name: useSubDomainName
  type: boolean
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-custom-domain-schema.json
slug: azure-storage-accounts-custom-domain
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: CustomDomain
---
