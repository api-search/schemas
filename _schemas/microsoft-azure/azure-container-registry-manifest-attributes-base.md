---
description: Manifest attribute details.
layout: schema
name: ManifestAttributesBase
properties_list:
- description: Manifest digest.
  name: digest
  type: string
- description: Image size.
  name: imageSize
  type: integer
- description: ''
  name: createdTime
  type: string
- description: ''
  name: lastUpdateTime
  type: string
- description: CPU architecture.
  name: architecture
  type: string
- description: Operating system.
  name: os
  type: string
- description: Media type.
  name: mediaType
  type: string
- description: Config media type.
  name: configMediaType
  type: string
- description: List of tags.
  name: tags
  type: array
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-manifest-attributes-base-schema.json
slug: azure-container-registry-manifest-attributes-base
source_filename: azure-container-registry-manifest-attributes-base-schema.json
source_heading: JSON Schema
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"ManifestAttributesBase\",\n  \"type\": \"object\",\n  \"description\": \"Manifest attribute details.\",\n  \"properties\": {\n    \"digest\": {\n      \"type\": \"string\",\n      \"description\": \"Manifest digest.\"\n    },\n    \"imageSize\": {\n      \"type\": \"integer\",\n      \"description\": \"Image size.\"\n    },\n    \"createdTime\": {\n      \"type\": \"string\"\n    },\n    \"lastUpdateTime\": {\n      \"type\": \"string\"\n    },\n    \"architecture\": {\n      \"type\": \"string\",\n      \"description\": \"CPU architecture.\"\n    },\n    \"os\": {\n      \"type\": \"string\",\n      \"description\": \"Operating system.\"\n    },\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"Media type.\"\n    },\n    \"configMediaType\": {\n      \"type\": \"string\",\n      \"description\": \"Config media type.\"\n    },\n    \"tags\": {\n      \"type\": \"array\"\
  ,\n      \"description\": \"List of tags.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-manifest-attributes-base-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: ManifestAttributesBase
---
