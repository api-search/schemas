---
description: An enumeration of blobs.
layout: schema
name: BlobEnumerationResults
properties_list:
- description: The service endpoint URL.
  name: ServiceEndpoint
  type: string
- description: The name of the container.
  name: ContainerName
  type: string
- description: The prefix used to filter results.
  name: Prefix
  type: string
- description: The marker used for pagination.
  name: Marker
  type: string
- description: The maximum number of results.
  name: MaxResults
  type: integer
- description: ''
  name: Blobs
  type: object
- description: The next marker for pagination.
  name: NextMarker
  type: string
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-blob-storage-blob-enumeration-results-schema.json
slug: azure-blob-storage-blob-enumeration-results
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"BlobEnumerationResults\",\n  \"type\": \"object\",\n  \"description\": \"An enumeration of blobs.\",\n  \"properties\": {\n    \"ServiceEndpoint\": {\n      \"type\": \"string\",\n      \"description\": \"The service endpoint URL.\"\n    },\n    \"ContainerName\": {\n      \"type\": \"string\",\n      \"description\": \"The name of the container.\"\n    },\n    \"Prefix\": {\n      \"type\": \"string\",\n      \"description\": \"The prefix used to filter results.\"\n    },\n    \"Marker\": {\n      \"type\": \"string\",\n      \"description\": \"The marker used for pagination.\"\n    },\n    \"MaxResults\": {\n      \"type\": \"integer\",\n      \"description\": \"The maximum number of results.\"\n    },\n    \"Blobs\": {\n      \"type\": \"object\"\n    },\n    \"NextMarker\": {\n      \"type\": \"string\",\n      \"description\": \"The next marker for pagination.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-blob-storage-blob-enumeration-results-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: BlobEnumerationResults
---
