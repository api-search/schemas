---
description: The List SAS credentials operation response.
layout: schema
name: ListAccountSasResponse
properties_list:
- description: List SAS credentials of storage account.
  name: accountSasToken
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-list-account-sas-response-schema.json
slug: azure-storage-accounts-list-account-sas-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-list-account-sas-response-schema.json\",\n  \"title\": \"ListAccountSasResponse\",\n  \"description\": \"The List SAS credentials operation response.\",\n  \"properties\": {\n    \"accountSasToken\": {\n      \"description\": \"List SAS credentials of storage account.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-list-account-sas-response-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ListAccountSasResponse
---
