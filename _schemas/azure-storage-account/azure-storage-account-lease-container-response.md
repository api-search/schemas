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
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-lease-container-response-schema.json
slug: azure-storage-account-lease-container-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-lease-container-response-schema.json\",\n  \"title\": \"LeaseContainerResponse\",\n  \"description\": \"Lease Container response schema.\",\n  \"properties\": {\n    \"leaseId\": {\n      \"description\": \"Returned unique lease ID that must be included with any request to delete the container, or to renew, change, or release the lease.\",\n      \"type\": \"string\"\n    },\n    \"leaseTimeSeconds\": {\n      \"description\": \"Approximate time remaining in the lease period, in seconds.\",\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-lease-container-response-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: LeaseContainerResponse
---
