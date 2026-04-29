---
description: A service that allows server-side encryption to be used.
layout: schema
name: EncryptionService
properties_list:
- description: A boolean indicating whether or not the service encrypts the data as it is stored.
  name: enabled
  type: boolean
- description: Encryption key type to be used for the encryption service. 'Account' key type implies that an account-scoped encryption key will be used. 'Service' key type implies that a default service key is used.
  name: keyType
  type: string
- description: Gets a rough estimate of the date/time when the encryption was last enabled by the user. Only returned when encryption is enabled. There might be some unencrypted blobs which were written after this t
  name: lastEnabledTime
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-encryption-service-schema.json
slug: azure-storage-account-encryption-service
source_filename: azure-storage-account-encryption-service-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-encryption-service-schema.json\",\n  \"title\": \"EncryptionService\",\n  \"description\": \"A service that allows server-side encryption to be used.\",\n  \"properties\": {\n    \"enabled\": {\n      \"description\": \"A boolean indicating whether or not the service encrypts the data as it is stored.\",\n      \"type\": \"boolean\"\n    },\n    \"keyType\": {\n      \"description\": \"Encryption key type to be used for the encryption service. 'Account' key type implies that an account-scoped encryption key will be used. 'Service' key type implies that a default service key is used.\",\n      \"enum\": [\n        \"Service\",\n        \"Account\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"KeyType\"\n\
  \      },\n      \"x-ms-mutability\": [\n        \"create\",\n        \"read\"\n      ]\n    },\n    \"lastEnabledTime\": {\n      \"description\": \"Gets a rough estimate of the date/time when the encryption was last enabled by the user. Only returned when encryption is enabled. There might be some unencrypted blobs which were written after this time, as it is just a rough estimate.\",\n      \"format\": \"date-time\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-encryption-service-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: EncryptionService
---
