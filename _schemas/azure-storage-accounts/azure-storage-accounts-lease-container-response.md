---
description: Lease Container response schema.
layout: schema
name: LeaseContainerResponse
properties_list:
- description: Returned unique lease ID that must be included with any request to delete the container, or to renew, change, or release the lease.
  name: leaseId
  type: string
- description: Approximate time remaining in the lease period, in seconds.
  name: leaseTimeSeconds
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-lease-container-response-schema.json
slug: azure-storage-accounts-lease-container-response
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: LeaseContainerResponse
---
