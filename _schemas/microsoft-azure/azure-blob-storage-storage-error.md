---
description: Storage service error response.
layout: schema
name: StorageError
properties_list:
- description: The error code.
  name: Code
  type: string
- description: The error message.
  name: Message
  type: string
- description: Additional details for authentication errors.
  name: AuthenticationErrorDetail
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-blob-storage-storage-error-schema.json
slug: azure-blob-storage-storage-error
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageError\",\n  \"type\": \"object\",\n  \"description\": \"Storage service error response.\",\n  \"properties\": {\n    \"Code\": {\n      \"type\": \"string\",\n      \"description\": \"The error code.\"\n    },\n    \"Message\": {\n      \"type\": \"string\",\n      \"description\": \"The error message.\"\n    },\n    \"AuthenticationErrorDetail\": {\n      \"type\": \"string\",\n      \"description\": \"Additional details for authentication errors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-blob-storage-storage-error-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: StorageError
---
