---
description: The URIs that are used to perform a retrieval of a public blob, queue, table, web or dfs object.
layout: schema
name: Endpoints
properties_list:
- description: Gets the blob endpoint.
  name: blob
  type: string
- description: Gets the dfs endpoint.
  name: dfs
  type: string
- description: Gets the file endpoint.
  name: file
  type: string
- description: Gets the internet routing storage endpoints
  name: internetEndpoints
  type: object
- description: Gets the microsoft routing storage endpoints.
  name: microsoftEndpoints
  type: object
- description: Gets the queue endpoint.
  name: queue
  type: string
- description: Gets the table endpoint.
  name: table
  type: string
- description: Gets the web endpoint.
  name: web
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-endpoints-schema.json
slug: azure-storage-account-endpoints
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: Endpoints
---
