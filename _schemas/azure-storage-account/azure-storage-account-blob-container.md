---
description: Properties of the blob container, including Id, resource name, resource type, Etag.
layout: schema
name: BlobContainer
properties_list:
- description: Properties of the blob container.
  name: properties
  type: object
provider_name: Azure Storage Account
provider_slug: azure-storage-account
schema_file: json-schema/azure-storage-account-blob-container-schema.json
slug: azure-storage-account-blob-container
source_filename: azure-storage-account-blob-container-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"$id\": \"https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-blob-container-schema.json\",\n  \"title\": \"BlobContainer\",\n  \"description\": \"Properties of the blob container, including Id, resource name, resource type, Etag.\",\n  \"properties\": {\n    \"properties\": {\n      \"$ref\": \"#/definitions/ContainerProperties\",\n      \"description\": \"Properties of the blob container.\",\n      \"x-ms-client-flatten\": true,\n      \"x-ms-client-name\": \"ContainerProperties\"\n    }\n  },\n  \"type\": \"object\"\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/azure-storage-account/refs/heads/main/json-schema/azure-storage-account-blob-container-schema.json
tags:
- Azure
- Blob Storage
- Cloud Storage
- File Storage
- Microsoft
- Storage
title: BlobContainer
---
