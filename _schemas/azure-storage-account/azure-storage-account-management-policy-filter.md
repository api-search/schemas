---
description: Filters limit rule actions to a subset of blobs within the storage account. If multiple filters are defined, a logical AND is performed on all filters.
layout: schema
name: ManagementPolicyFilter
properties_list:
- description: An array of predefined enum values. Only blockBlob is supported.
  name: blobTypes
  type: array
- description: An array of strings for prefixes to be match.
  name: prefixMatch
  type: array
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-management-policy-filter-schema.json
slug: azure-storage-account-management-policy-filter
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ManagementPolicyFilter
---
