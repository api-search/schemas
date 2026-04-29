---
description: The encryption settings on the storage account.
layout: schema
name: Encryption
properties_list:
- description: 'The encryption keySource (provider). Possible values (case-insensitive): Microsoft.Storage, Microsoft.Keyvault'
  name: keySource
  type: string
- description: Properties provided by key vault.
  name: keyvaultproperties
  type: object
- description: List of services which support encryption.
  name: services
  type: object
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-encryption-schema.json
slug: azure-storage-accounts-encryption
source_filename: azure-storage-accounts-encryption-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-encryption-schema.json\",\n  \"title\": \"Encryption\",\n  \"description\": \"The encryption settings on the storage account.\",\n  \"properties\": {\n    \"keySource\": {\n      \"default\": \"Microsoft.Storage\",\n      \"description\": \"The encryption keySource (provider). Possible values (case-insensitive):  Microsoft.Storage, Microsoft.Keyvault\",\n      \"enum\": [\n        \"Microsoft.Storage\",\n        \"Microsoft.Keyvault\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": true,\n        \"name\": \"KeySource\"\n      }\n    },\n    \"keyvaultproperties\": {\n      \"$ref\": \"#/definitions/KeyVaultProperties\",\n      \"description\": \"Properties provided by key vault.\",\n      \"x-ms-client-name\": \"KeyVaultProperties\"\
  \n    },\n    \"services\": {\n      \"$ref\": \"#/definitions/EncryptionServices\",\n      \"description\": \"List of services which support encryption.\"\n    }\n  },\n  \"type\": \"object\",\n  \"required\": [\n    \"keySource\"\n  ]\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-encryption-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: Encryption
---
