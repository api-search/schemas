---
description: Docker V2 image layer descriptor.
layout: schema
name: Descriptor
properties_list:
- description: Layer media type.
  name: mediaType
  type: string
- description: Layer size.
  name: size
  type: integer
- description: Layer digest.
  name: digest
  type: string
- description: Specifies a list of URLs from which this object may be downloaded.
  name: urls
  type: array
- description: Additional information about the descriptor.
  name: annotations
  type: object
provider_name: Microsoft Azure
provider_slug: microsoft-azure
schema_file: json-schema/azure-container-registry-descriptor-schema.json
slug: azure-container-registry-descriptor
source_json: "{\n  \"$schema\": \"https://json-schema.org/draft/2020-12/schema\",\n  \"title\": \"Descriptor\",\n  \"type\": \"object\",\n  \"description\": \"Docker V2 image layer descriptor.\",\n  \"properties\": {\n    \"mediaType\": {\n      \"type\": \"string\",\n      \"description\": \"Layer media type.\"\n    },\n    \"size\": {\n      \"type\": \"integer\",\n      \"description\": \"Layer size.\"\n    },\n    \"digest\": {\n      \"type\": \"string\",\n      \"description\": \"Layer digest.\"\n    },\n    \"urls\": {\n      \"type\": \"array\",\n      \"description\": \"Specifies a list of URLs from which this object may be downloaded.\"\n    },\n    \"annotations\": {\n      \"type\": \"object\",\n      \"description\": \"Additional information about the descriptor.\"\n    }\n  }\n}"
source_json_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure/refs/heads/main/json-schema/azure-container-registry-descriptor-schema.json
tags:
- API Management
- Cloud
- Cloud Computing
- Enterprise
- Infrastructure as a Service
- Platform as a Service
- T1
title: Descriptor
---
