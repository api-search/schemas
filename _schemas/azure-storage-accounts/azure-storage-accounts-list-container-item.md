---
description: The blob container properties be listed out.
layout: schema
name: ListContainerItem
properties_list:
- description: The blob container properties be listed out.
  name: properties
  type: object
provider_name: Azure Storage Accounts
provider_slug: azure-storage-accounts
schema_file: json-schema/azure-storage-accounts-list-container-item-schema.json
slug: azure-storage-accounts-list-container-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-list-container-item-schema.json\",\n  \"title\": \"ListContainerItem\",\n  \"description\": \"The blob container properties be listed out.\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/ContainerProperties\",\n      \"description\": \"The blob container properties be listed out.\",\n      \"x-ms-client-flatten\": true\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-accounts/refs/heads/main/json-schema/azure-storage-accounts-list-container-item-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Queue Storage
- Storage
- Table Storage
title: ListContainerItem
---
