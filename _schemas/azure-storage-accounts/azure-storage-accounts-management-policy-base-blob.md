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
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-management-policy-base-blob-schema.json\",\n  \"title\": \"ManagementPolicyBaseBlob\",\n  \"description\": \"Management policy action for base blob.\",\n  \"properties\": {\n    \"delete\": {\n      \"$ref\": \"#/definitions/DateAfterModification\",\n      \"description\": \"The function to delete the blob\"\n    },\n    \"tierToArchive\": {\n      \"$ref\": \"#/definitions/DateAfterModification\",\n      \"description\": \"The function to tier blobs to archive storage. Support blobs currently at Hot or Cool tier\"\n    },\n    \"tierToCool\": {\n      \"$ref\": \"#/definitions/DateAfterModification\",\n      \"description\": \"The function to tier blobs to cool storage. Support blobs currently at Hot tier\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-management-policy-base-blob-schema.json
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
