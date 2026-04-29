---
description: Properties of a blob.
layout: schema
name: BlobProperties
properties_list:
- description: The date/time the blob was created.
  name: Creation-Time
  type: string
- description: The date/time the blob was last modified.
  name: Last-Modified
  type: string
- description: The ETag of the blob.
  name: Etag
  type: string
- description: The size of the blob in bytes.
  name: Content-Length
  type: integer
- description: The content type of the blob.
  name: Content-Type
  type: string
- description: The content encoding of the blob.
  name: Content-Encoding
  type: string
- description: The content language of the blob.
  name: Content-Language
  type: string
- description: The MD5 hash of the blob content.
  name: Content-MD5
  type: string
- description: The content disposition of the blob.
  name: Content-Disposition
  type: string
- description: The cache control of the blob.
  name: Cache-Control
  type: string
- description: The type of the blob.
  name: BlobType
  type: string
- description: The access tier of the blob.
  name: AccessTier
  type: string
- description: Whether the access tier was inferred.
  name: AccessTierInferred
  type: boolean
- description: The lease status.
  name: LeaseStatus
  type: string
- description: The lease state.
  name: LeaseState
  type: string
- description: Whether the blob data and metadata are encrypted.
  name: ServerEncrypted
  type: boolean
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-blob-storage-blob-properties-schema.json
slug: azure-blob-storage-blob-properties
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlobProperties\",\n  \"type\": \"object\",\n  \"description\": \"Properties of a blob.\",\n  \"properties\": {\n    \"Creation-Time\": {\n      \"type\": \"string\",\n      \"description\": \"The date/time the blob was created.\"\n    },\n    \"Last-Modified\": {\n      \"type\": \"string\",\n      \"description\": \"The date/time the blob was last modified.\"\n    },\n    \"Etag\": {\n      \"type\": \"string\",\n      \"description\": \"The ETag of the blob.\"\n    },\n    \"Content-Length\": {\n      \"type\": \"integer\",\n      \"description\": \"The size of the blob in bytes.\"\n    },\n    \"Content-Type\": {\n      \"type\": \"string\",\n      \"description\": \"The content type of the blob.\"\n    },\n    \"Content-Encoding\": {\n      \"type\": \"string\",\n      \"description\": \"The content encoding of the blob.\"\n    },\n    \"Content-Language\": {\n      \"type\": \"string\"\
  ,\n      \"description\": \"The content language of the blob.\"\n    },\n    \"Content-MD5\": {\n      \"type\": \"string\",\n      \"description\": \"The MD5 hash of the blob content.\"\n    },\n    \"Content-Disposition\": {\n      \"type\": \"string\",\n      \"description\": \"The content disposition of the blob.\"\n    },\n    \"Cache-Control\": {\n      \"type\": \"string\",\n      \"description\": \"The cache control of the blob.\"\n    },\n    \"BlobType\": {\n      \"type\": \"string\",\n      \"description\": \"The type of the blob.\"\n    },\n    \"AccessTier\": {\n      \"type\": \"string\",\n      \"description\": \"The access tier of the blob.\"\n    },\n    \"AccessTierInferred\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the access tier was inferred.\"\n    },\n    \"LeaseStatus\": {\n      \"type\": \"string\",\n      \"description\": \"The lease status.\"\n    },\n    \"LeaseState\": {\n      \"type\": \"string\",\n      \"description\": \"The\
  \ lease state.\"\n    },\n    \"ServerEncrypted\": {\n      \"type\": \"boolean\",\n      \"description\": \"Whether the blob data and metadata are encrypted.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-blob-storage-blob-properties-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: BlobProperties
---
