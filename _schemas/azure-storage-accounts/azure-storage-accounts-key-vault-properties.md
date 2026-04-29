---
description: Properties of key vault.
layout: schema
name: KeyVaultProperties
properties_list:
- description: The name of KeyVault key.
  name: keyname
  type: string
- description: The Uri of KeyVault.
  name: keyvaulturi
  type: string
- description: The version of KeyVault key.
  name: keyversion
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-key-vault-properties-schema.json
slug: azure-storage-accounts-key-vault-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-key-vault-properties-schema.json\",\n  \"title\": \"KeyVaultProperties\",\n  \"description\": \"Properties of key vault.\",\n  \"properties\": {\n    \"keyname\": {\n      \"description\": \"The name of KeyVault key.\",\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"KeyName\"\n    },\n    \"keyvaulturi\": {\n      \"description\": \"The Uri of KeyVault.\",\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"KeyVaultUri\"\n    },\n    \"keyversion\": {\n      \"description\": \"The version of KeyVault key.\",\n      \"type\": \"string\",\n      \"x-ms-client-name\": \"KeyVersion\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-key-vault-properties-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: KeyVaultProperties
---
