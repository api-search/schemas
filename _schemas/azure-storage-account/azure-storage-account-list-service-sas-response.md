---
description: The List service SAS credentials operation response.
layout: schema
name: ListServiceSasResponse
properties_list:
- description: List service SAS credentials of specific resource.
  name: serviceSasToken
  type: string
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-list-service-sas-response-schema.json
slug: azure-storage-account-list-service-sas-response
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-list-service-sas-response-schema.json\",\n  \"title\": \"ListServiceSasResponse\",\n  \"description\": \"The List service SAS credentials operation response.\",\n  \"properties\": {\n    \"serviceSasToken\": {\n      \"description\": \"List service SAS credentials of specific resource.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-list-service-sas-response-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: ListServiceSasResponse
---
