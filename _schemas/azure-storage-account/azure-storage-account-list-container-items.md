---
description: Response schema. Contains list of blobs returned, and if paging is requested or required, a URL to next page of containers.
layout: schema
name: ListContainerItems
properties_list:
- description: Request URL that can be used to query next page of containers. Returned when total number of requested containers exceed maximum page size.
  name: nextLink
  type: string
- description: List of blobs containers returned.
  name: value
  type: array
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-list-container-items-schema.json
slug: azure-storage-account-list-container-items
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ListContainerItems
---
