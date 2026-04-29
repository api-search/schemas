---
description: Azure Files or Blob Storage access information value for dictionary storage.
layout: schema
name: AzureStorageInfoValue
properties_list:
- description: Access key for the storage account.
  name: accessKey
  type: string
- description: Name of the storage account.
  name: accountName
  type: string
- description: Path to mount the storage within the site's runtime environment.
  name: mountPath
  type: string
- description: Name of the file share (container name, for Blob storage).
  name: shareName
  type: string
- description: State of the storage account.
  name: state
  type: string
- description: Type of storage.
  name: type
  type: string
provider_name: Azure Functions
provider_slug: azure-functions
schema_file: json-schema/azure-functions-azure-storage-info-value-schema.json
slug: azure-functions-azure-storage-info-value
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-azure-storage-info-value-schema.json\",\n  \"title\": \"AzureStorageInfoValue\",\n  \"description\": \"Azure Files or Blob Storage access information value for dictionary storage.\",\n  \"type\": \"object\",\n  \"properties\": {\n    \"accessKey\": {\n      \"description\": \"Access key for the storage account.\",\n      \"type\": \"string\"\n    },\n    \"accountName\": {\n      \"description\": \"Name of the storage account.\",\n      \"type\": \"string\"\n    },\n    \"mountPath\": {\n      \"description\": \"Path to mount the storage within the site's runtime environment.\",\n      \"type\": \"string\"\n    },\n    \"shareName\": {\n      \"description\": \"Name of the file share (container name, for Blob storage).\",\n      \"type\": \"string\"\n    },\n    \"state\": {\n      \"description\"\
  : \"State of the storage account.\",\n      \"enum\": [\n        \"Ok\",\n        \"InvalidCredentials\",\n        \"InvalidShare\"\n      ],\n      \"readOnly\": true,\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"AzureStorageState\"\n      }\n    },\n    \"type\": {\n      \"description\": \"Type of storage.\",\n      \"enum\": [\n        \"AzureFiles\",\n        \"AzureBlob\"\n      ],\n      \"type\": \"string\",\n      \"x-ms-enum\": {\n        \"modelAsString\": false,\n        \"name\": \"AzureStorageType\"\n      }\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-functions/refs/heads/main/json-schema/azure-functions-azure-storage-info-value-schema.json
tags:
- Cloud
- Compute
- Event-Driven
- Functions
- Serverless
title: AzureStorageInfoValue
---
