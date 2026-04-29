---
description: Storage service properties.
layout: schema
name: StorageServiceProperties
properties_list:
- description: Azure Analytics logging settings.
  name: Logging
  type: object
- description: The set of CORS rules.
  name: Cors
  type: object
- description: The default version to use for requests to the Blob service.
  name: DefaultServiceVersion
  type: string
- description: The properties that enable static website hosting.
  name: StaticWebsite
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-blob-storage-storage-service-properties-schema.json
slug: azure-blob-storage-storage-service-properties
source_filename: azure-blob-storage-storage-service-properties-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"StorageServiceProperties\",\n  \"type\": \"object\",\n  \"description\": \"Storage service properties.\",\n  \"properties\": {\n    \"Logging\": {\n      \"type\": \"object\",\n      \"description\": \"Azure Analytics logging settings.\"\n    },\n    \"Cors\": {\n      \"type\": \"object\",\n      \"description\": \"The set of CORS rules.\"\n    },\n    \"DefaultServiceVersion\": {\n      \"type\": \"string\",\n      \"description\": \"The default version to use for requests to the Blob service.\"\n    },\n    \"StaticWebsite\": {\n      \"type\": \"object\",\n      \"description\": \"The properties that enable static website hosting.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-blob-storage-storage-service-properties-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: StorageServiceProperties
---
