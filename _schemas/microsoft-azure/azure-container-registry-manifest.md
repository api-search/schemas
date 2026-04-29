---
description: Docker V2 manifest.
layout: schema
name: Manifest
properties_list:
- description: Schema version.
  name: schemaVersion
  type: integer
- description: Media type.
  name: mediaType
  type: string
- description: List of layer descriptors.
  name: layers
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-manifest-schema.json
slug: azure-container-registry-manifest
source_filename: azure-container-registry-manifest-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Manifest\",\n  \"type\": \"object\",\n  \"description\": \"Docker V2 manifest.\",\n  \"properties\": {\n    \"schemaVersion\": {\n      \"type\": \"integer\",\n      \"description\": \"Schema version.\"\n    },\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"Media type.\"\n    },\n    \"layers\": {\n      \"type\": \"array\",\n      \"description\": \"List of layer descriptors.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-manifest-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Manifest
---
