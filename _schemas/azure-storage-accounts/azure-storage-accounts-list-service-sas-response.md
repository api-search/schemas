---
description: The List service SAS credentials operation response.
layout: schema
name: ListServiceSasResponse
properties_list:
- description: List service SAS credentials of specific resource.
  name: serviceSasToken
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-list-service-sas-response-schema.json
slug: azure-storage-accounts-list-service-sas-response
source_filename: azure-storage-accounts-list-service-sas-response-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-list-service-sas-response-schema.json\",\n  \"title\": \"ListServiceSasResponse\",\n  \"description\": \"The List service SAS credentials operation response.\",\n  \"properties\": {\n    \"serviceSasToken\": {\n      \"description\": \"List service SAS credentials of specific resource.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-list-service-sas-response-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ListServiceSasResponse
---
