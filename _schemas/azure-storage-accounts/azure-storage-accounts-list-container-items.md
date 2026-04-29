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
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-list-container-items-schema.json
slug: azure-storage-accounts-list-container-items
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-list-container-items-schema.json\",\n  \"title\": \"ListContainerItems\",\n  \"description\": \"Response schema. Contains list of blobs returned, and if paging is requested or required, a URL to next page of containers.\",\n  \"properties\": {\n    \"nextLink\": {\n      \"description\": \"Request URL that can be used to query next page of containers. Returned when total number of requested containers exceed maximum page size.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"value\": {\n      \"description\": \"List of blobs containers returned.\",\n      \"items\": {\n        \"$ref\": \"#/definitions/ListContainerItem\"\n      },\n      \"readOnly\": true,\n      \"type\": \"array\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-list-container-items-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ListContainerItems
---
