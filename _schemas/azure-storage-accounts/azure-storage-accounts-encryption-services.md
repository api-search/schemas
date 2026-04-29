---
description: A list of services that support encryption.
layout: schema
name: EncryptionServices
properties_list:
- description: The encryption function of the blob storage service.
  name: blob
  type: object
- description: The encryption function of the file storage service.
  name: file
  type: object
- description: The encryption function of the queue storage service.
  name: queue
  type: object
- description: The encryption function of the table storage service.
  name: table
  type: object
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-encryption-services-schema.json
slug: azure-storage-accounts-encryption-services
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-encryption-services-schema.json\",\n  \"title\": \"EncryptionServices\",\n  \"description\": \"A list of services that support encryption.\",\n  \"properties\": {\n    \"blob\": {\n      \"$ref\": \"#/definitions/EncryptionService\",\n      \"description\": \"The encryption function of the blob storage service.\"\n    },\n    \"file\": {\n      \"$ref\": \"#/definitions/EncryptionService\",\n      \"description\": \"The encryption function of the file storage service.\"\n    },\n    \"queue\": {\n      \"$ref\": \"#/definitions/EncryptionService\",\n      \"description\": \"The encryption function of the queue storage service.\"\n    },\n    \"table\": {\n      \"$ref\": \"#/definitions/EncryptionService\",\n      \"description\": \"The encryption function of the table storage\
  \ service.\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-encryption-services-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: EncryptionServices
---
