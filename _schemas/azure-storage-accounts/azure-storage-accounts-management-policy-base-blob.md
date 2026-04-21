---
description: Management policy action for base blob.
layout: schema
name: ManagementPolicyBaseBlob
properties_list:
- description: The function to delete the blob
  name: delete
  type: object
- description: The function to tier blobs to archive storage. Support blobs currently at Hot or Cool tier
  name: tierToArchive
  type: object
- description: The function to tier blobs to cool storage. Support blobs currently at Hot tier
  name: tierToCool
  type: object
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-management-policy-base-blob-schema.json
slug: azure-storage-accounts-management-policy-base-blob
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ManagementPolicyBaseBlob
---
