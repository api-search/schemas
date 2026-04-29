---
description: The URIs that are used to perform a retrieval of a public blob, queue, table, web or dfs object.
layout: schema
name: Endpoints
properties_list:
- description: Gets the blob endpoint.
  name: blob
  type: string
- description: Gets the dfs endpoint.
  name: dfs
  type: string
- description: Gets the file endpoint.
  name: file
  type: string
- description: Gets the internet routing storage endpoints
  name: internetEndpoints
  type: object
- description: Gets the microsoft routing storage endpoints.
  name: microsoftEndpoints
  type: object
- description: Gets the queue endpoint.
  name: queue
  type: string
- description: Gets the table endpoint.
  name: table
  type: string
- description: Gets the web endpoint.
  name: web
  type: string
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-endpoints-schema.json
slug: azure-storage-accounts-endpoints
source_filename: azure-storage-accounts-endpoints-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-endpoints-schema.json\",\n  \"title\": \"Endpoints\",\n  \"description\": \"The URIs that are used to perform a retrieval of a public blob, queue, table, web or dfs object.\",\n  \"properties\": {\n    \"blob\": {\n      \"description\": \"Gets the blob endpoint.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"dfs\": {\n      \"description\": \"Gets the dfs endpoint.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"file\": {\n      \"description\": \"Gets the file endpoint.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"internetEndpoints\": {\n      \"$ref\": \"#/definitions/StorageAccountInternetEndpoints\",\n      \"description\": \"Gets the internet routing storage endpoints\",\n      \"x-ms-client-flatten\"\
  : false\n    },\n    \"microsoftEndpoints\": {\n      \"$ref\": \"#/definitions/StorageAccountMicrosoftEndpoints\",\n      \"description\": \"Gets the microsoft routing storage endpoints.\",\n      \"x-ms-client-flatten\": false\n    },\n    \"queue\": {\n      \"description\": \"Gets the queue endpoint.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"table\": {\n      \"description\": \"Gets the table endpoint.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    },\n    \"web\": {\n      \"description\": \"Gets the web endpoint.\",\n      \"readOnly\": true,\n      \"type\": \"string\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-endpoints-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: Endpoints
---
