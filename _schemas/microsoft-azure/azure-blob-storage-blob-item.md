---
description: A blob item in the enumeration results.
layout: schema
name: BlobItem
properties_list:
- description: The name of the blob.
  name: Name
  type: string
- description: Whether the blob is deleted.
  name: Deleted
  type: boolean
- description: The snapshot DateTime.
  name: Snapshot
  type: string
- description: The version ID of the blob.
  name: VersionId
  type: string
- description: Whether this is the current version.
  name: IsCurrentVersion
  type: boolean
- description: The blob metadata.
  name: Metadata
  type: object
- description: Blob tags.
  name: Tags
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-blob-storage-blob-item-schema.json
slug: azure-blob-storage-blob-item
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlobItem\",\n  \"type\": \"object\",\n  \"description\": \"A blob item in the enumeration results.\",\n  \"properties\": {\n    \"Name\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the blob.\"\n    },\n    \"Deleted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the blob is deleted.\"\n    },\n    \"Snapshot\": {\n      \"type\": \"string\",\n      \"description\": \"The snapshot DateTime.\"\n    },\n    \"VersionId\": {\n      \"type\": \"string\",\n      \"description\": \"The version ID of the blob.\"\n    },\n    \"IsCurrentVersion\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether this is the current version.\"\n    },\n    \"Metadata\": {\n      \"type\": \"object\",\n      \"description\": \"The blob metadata.\"\n    },\n    \"Tags\": {\n      \"type\": \"object\",\n      \"description\": \"Blob tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-blob-storage-blob-item-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: BlobItem
---
